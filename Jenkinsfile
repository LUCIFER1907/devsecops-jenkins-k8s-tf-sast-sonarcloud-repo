pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=allen-buggy-app -Dsonar.organization=Allen_Buggy_App -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=d3ab23d55facb161b3f97eec6d87c8c384cd38b1'
			}
        } 
  }
}
