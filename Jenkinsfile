pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=bugwebappdevsecops -Dsonar.organization=bugwebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=62bacbc5aa5f74d64be3df243fcfdb318e908e1d'
			}
        } 
  }
}
