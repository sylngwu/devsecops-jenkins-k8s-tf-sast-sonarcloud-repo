pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=ebukadevsecopsbuggywebapp -Dsonar.organization=ebukadevsecopsbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=d11254d304859f3914c00750be373910e30f5c91'
			}
        } 
  }
}
