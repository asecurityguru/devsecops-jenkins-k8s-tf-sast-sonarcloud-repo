pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify org.sonarsource.scanner.maven:sonar-maven-plugin:sonar -Dsonar.projectKey=akbuggywebapp -Dsonar.organization=testoneado -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=da6b417159cbb17a1f0f5f258b6a1c62dd096899'
			}
        } 
  }
}
