pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=awsbuggywebapp -Dsonar.organization=awsbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=df3e2e923185af82dcea682e9362e8bdaaa02347'
			}
        } 
  }
}
