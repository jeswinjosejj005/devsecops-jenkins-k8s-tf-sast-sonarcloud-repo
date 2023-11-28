pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=securityudemy -Dsonar.organization=securityudemy -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=c68440e6deff73c181a6d628c1c6d7c76c4c2db9'
			}
        } 
  }
}
