pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecopslab2023 -Dsonar.organization=DevSecOps -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=c907112fee00ceeabc0c133ecb1fbf0eb6462e31'
			}
        } 
  }
}
