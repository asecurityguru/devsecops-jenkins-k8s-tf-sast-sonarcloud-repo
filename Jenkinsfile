pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=Abrahamitjob -Dsonar.organization=Abrahamitjob -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=91bbcc85e5ae3bf8c463dcbfed2743e2cfc31a71'
			}
        } 
  }
}
