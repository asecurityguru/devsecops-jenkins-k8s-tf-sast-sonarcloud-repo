pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=cybharathetabuggywebapp -Dsonar.organization=cybharathetabuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=e3e50ed961b654da8893edd516ade02221041bdd'
			}
        } 
  }
}
