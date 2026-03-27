pipeline {
  agent any
  tools { 
        maven 'Maven_3_8_4'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=Maxeebuggytoken -Dsonar.organization=Maxeebuggytoken -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=736a7e0dbeec793bd8d9474978f25fed8ed55d7b'
			}
        } 
  }
}
