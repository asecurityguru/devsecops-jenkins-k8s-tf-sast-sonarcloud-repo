pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=djcliffmixwebapp -Dsonar.organization=djcliffmixwebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=f2480ae5ce4c89ca999021debbc7bc421f172219'
			}
        } 
  }
}
