pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp -Dsonar.organization=asgbuggywebap -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=b58c9ba1c0530a2a501db8533d4df46ec7b1951a'
			}
        } 
  }
}
