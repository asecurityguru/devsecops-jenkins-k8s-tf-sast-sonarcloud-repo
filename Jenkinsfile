pipeline {
  agent any
  tools { 
        maven 'Maven_3_8_4'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=ramdev233 -Dsonar.organization=RamDev -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=901858f2bee86f0c6d0253a8ec03b961edb2ebd6'
			}
        } 
  }
}
