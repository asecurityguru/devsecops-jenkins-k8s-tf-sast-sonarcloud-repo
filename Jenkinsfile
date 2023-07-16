pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=f-ahmed -Dsonar.organization=f-ahmed -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=2f3b32f228ab3098d94d48ce04948d7309c9d3cf'
			}
        } 
  }
}
