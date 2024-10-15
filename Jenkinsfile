pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=buggywebapportest -Dsonar.organization=DevSecOpsKurs -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=9bd5ed63b7e36b38bbe8e9df4998da40ee05f764d'
			}
        } 
  }
}
