pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=buggywebapp-1 -Dsonar.organization=asgbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=51e7f70f19df8fa36b336ea37c217f2c3998c154'
			}
        } 
  }
}
