pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=projectKey -Dsonar.organization=organizationKey -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=sonarToken'
			}
        } 
  }
}
