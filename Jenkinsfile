pipeline {
  agent any
  tools { 
        maven 'Maven_3_8_4'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify org.sonarsource.scanner.maven:sonar-maven-plugin:sonar -Dsonar.projectKey=devopsak_devopsak -Dsonar.organization=devopsak -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=2300de2068a9bd5e16d63a063c42cda3d27f2ecb'
			}
        } 
  }
}
