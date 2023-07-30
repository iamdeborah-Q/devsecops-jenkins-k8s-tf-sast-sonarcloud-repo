pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=terraformwebapp_terraformwebapp -Dsonar.organization=terraformwebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=9035649de4fa027cd9d1d88caf83c37017fa044a'
			}
        } 
  }
}
