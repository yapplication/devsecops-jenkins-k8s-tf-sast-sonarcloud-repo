pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=ysonarcloud -Dsonar.organization=ysonarcloud -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=55f9800b4a6a48584a4bbb13112662ece950e65a'
			}
        } 
  }
}
