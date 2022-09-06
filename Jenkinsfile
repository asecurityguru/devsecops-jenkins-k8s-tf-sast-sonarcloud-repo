pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage ('run maven') {
      steps {
            sh 'mvn clean package -Dmaven.test.skip=true'     
      }
    }
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn -Dmaven.test.failure.ignore verify sonar:sonar -Dsonar.projectKey=projectKey -Dsonar.organization=organizationKey -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=sonarToken'
			}
        } 
  }
}
