pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=shishirbuggywebapp -Dsonar.organization=shishirbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=507d0a225078ecd8f3938268a3db6197b4539691'
			}
        } 
  }
}
