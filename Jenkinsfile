pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=buggynew -Dsonar.organization=buggy -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=8bd777ad1362584be36047e1fe058b3dd62e0d28'
			}
        } 
  }
}
