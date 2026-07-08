pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebappjkjd_asgbuggywebappjkjd -Dsonar.organization=asgbuggywebappjkjd -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=bdc7dd390765a5e9ec7b8fa8d637a5999a215f8a'
			}
        } 
  }
}
