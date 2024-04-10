pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=allen-buggy-app -Dsonar.organization=Allen_Buggy_App -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=7ae85416627e27831f8612e6bd894122dfb5ae41'
			}
        } 
  }
}
