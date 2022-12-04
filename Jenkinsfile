pipeline {
  agent any
  tools { 
        maven 'Maven_3_6_3'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=smdemo -Dsonar.organization=setth -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=f6fc24f42103facc3402fdd5a39b0ccec8ea0444'
			}
        } 
  }
}
