pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecops -Dsonar.organization=devsecops -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=c762597408438a529cd7f9964fbfca7ab3c6e875'
			}
        } 
  }
}
