pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asecuritybugywebapp -Dsonar.organization=asecuritybugywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=e462b79684f41c177e55e66a7c0a1452d713f745'
			}
        } 
  }
}
