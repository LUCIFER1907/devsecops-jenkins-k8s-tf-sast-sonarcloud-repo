pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=allenbuggwebapp -Dsonar.organization=allenbuggwebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=5bcb880d19beebdfaddb67a7172f29c9b15f326a'
			}
        } 
  }
}
