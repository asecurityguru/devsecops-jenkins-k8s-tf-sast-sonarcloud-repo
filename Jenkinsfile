pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify org.sonarsource.scanner.maven:sonar-maven-plugin:sonar -Dsonar.projectKey=omdev -Dsonar.organization=omdev -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=33ed98f27f645689fcd67d18a23dcc9aa3476546'
			}
        } 
  }
}
