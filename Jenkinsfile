pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecopswebbapp -Dsonar.organization=devsecopswebbapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=97287d28b353ca37314b31d81b37148b94b97565'
			}
        } 
  }
}
