pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=secureat -Dsonar.organization=secureat -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=4882d4db1992823217297af68445ebc1f5dfb3e8'
			}
        } 
  }
}
