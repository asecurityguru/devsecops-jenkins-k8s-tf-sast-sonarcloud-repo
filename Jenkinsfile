pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp10 -Dsonar.organization=asgbuggywebapp10 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=c8d30e20cbdbeafa587e1481398696f8b65cf1cc'
			}
        }
	stage('RunSCAAnalysisUsingSnyk') {
            steps {
				withCredentials([string(credentialsId: 'SNYK_TOKEN', variable: 'SNYK_TOKEN')]) {
					sh 'mvn snyk:test -fn'
				}
			}
    }

	stage('Build') {
            steps {
               withDockerRegistry([credentialsId: "dockerlogin", url: ""]) {
                 script {
                    app =  docker.build("lnb")
                 }
               }
            }
    }

	stage('Push') {
            steps {
                script {
                    docker.withRegistry('https://363981201235.dkr.ecr.us-west-2.amazonaws.com', 'ecr:us-west-2:aws-credentials') {
                        app.push("latest")
                    }
                }
            }
    }
}