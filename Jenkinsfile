pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=navinbuggyapp -Dsonar.organization=navinbuggyapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=66196745226df0a6d6b2d461701925dcd1bb5749'
			}
        } 
  }
}
