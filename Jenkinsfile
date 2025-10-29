pipeline {
  agent any
  tools { 
        maven 'Maven_3_8_4'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {		
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=Shaik2310 -Dsonar.organization=Shaik2310 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=79b214def18eee4a19d5f5067f9b577fbb7aac60'
			}
        } 
  }
}
