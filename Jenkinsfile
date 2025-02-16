pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devbuggywebapp -Dsonar.organization=devanshu -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=c15085f7f06ff18862a805d1b858d4bf059bdae4'
			}
        } 
  }
}
