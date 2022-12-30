pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgburgywebapp -Dsonar.organization=asgburgywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=030dbf8a10f398309760a8b8556b324e71df04eb'
			}
        } 
  }
}
