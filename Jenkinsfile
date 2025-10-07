pipeline {
  agent any
  tools { 
        maven 'Maven_3_8_4'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecops682_devsecops682 -Dsonar.organization=devsecops682 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=6f7aff123ac3555e37c64df5d63cd42166609231'
			}
        } 
  }
}
