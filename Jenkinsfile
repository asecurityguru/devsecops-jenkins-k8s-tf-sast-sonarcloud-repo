pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify org.sonarsource.scanner.maven:sonar-maven-plugin:sonar -Dsonar.projectKey=testoneado -Dsonar.organization=testoneado -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=0716ab3bd8d2d91a743a49cb07f61546fadbfcf3'
			}
        } 
  }
}
