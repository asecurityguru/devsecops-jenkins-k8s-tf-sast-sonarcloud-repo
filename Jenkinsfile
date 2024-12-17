pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=ashbugwebapp -Dsonar.organization=ashbugwebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=7a17ca2272a64f86bda652048416c1dfdee7b73e'
			}
        } 
  }
}
