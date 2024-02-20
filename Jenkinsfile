pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asecuritybugywebapp -Dsonar.organization=asecuritybugywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=c22b0ae52117e48304494152f3c8946913ba5a15'
			}
        } 
  }
}
