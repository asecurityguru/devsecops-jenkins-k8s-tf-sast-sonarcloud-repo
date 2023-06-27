pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp10 -Dsonar.organization=asgbuggywebapp10 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=c8d30e20cbdbeafa587e1481398696f8b65cf1cc'
			}
        } 
  }
}
