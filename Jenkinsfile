pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=bumbum -Dsonar.organization=bumbum -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=c6753dfa0815a1109d8d66181e962b0505e5cbde'
			}
        } 
  }
}
