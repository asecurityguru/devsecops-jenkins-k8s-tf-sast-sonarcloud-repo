pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=absecuritybuggywebapp -Dsonar.organization=absecuritybuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=7e28d2d882ef0ae43f3655c6e7c1ae6abda2ae8f'
			}
        } 
  }
}
