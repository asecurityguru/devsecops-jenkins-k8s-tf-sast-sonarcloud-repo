pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=thomaslifedesign -Dsonar.organization=thomaslifedesign -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=12c45897f4f4c1842dce9f7ece58e31c3d776b3e'
			}
        } 
  }
}
