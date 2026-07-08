pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=mohanabuggyapp_mohanabuggyapp -Dsonar.organization=mohanabuggyapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=2edbe6301c281a6fd68eccdb66d1fea2603d4d9c'
			}
        } 
  }
}
