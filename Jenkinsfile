pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=nakiba -Dsonar.organization=nakiba -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=be75d7b17946ef42686598a22065e2007a2eff5a'
			}
        } 
  }
}
