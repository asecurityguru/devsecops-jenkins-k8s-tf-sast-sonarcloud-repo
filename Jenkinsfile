pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=csecuritybuggyapp -Dsonar.organization=csecuritybuggyapp
 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=c06f7da82db09b022cc90179086a95af663e06db'
			}
        } 
  }
}
