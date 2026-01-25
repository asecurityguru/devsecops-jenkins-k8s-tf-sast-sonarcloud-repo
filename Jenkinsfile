pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=ebuggywebapp -Dsonar.organization=ebuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=6eb52be728f0fb3e8b90d40b0bdd28a979131f7b9'
			}
        } 
  }
}
