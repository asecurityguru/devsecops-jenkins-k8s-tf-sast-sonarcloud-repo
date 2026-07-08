pipeline {
  agent any
  tools { 
        maven 'Maven_3.2.5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=chetnawangnoo -Dsonar.organization=chetnawangnoo -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=123851c285f16eef0732c84e90185cacfc2900e3'
			}
        } 
  }
}
