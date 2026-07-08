pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=buggyapp-praveen -Dsonar.organization=BuggyApp_Praveen -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=6d93509208f02d3abf44d0a371918ca5f5066ff2'
			}
        } 
  }
}
