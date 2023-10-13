pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp1233 -Dsonar.organization=asgbuggywebapp1233 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=fcc83e2a9b82e39337d5bb0e250f72ab1de60309'
			}
        } 
  }
}
