pipeline {
  agent any
  tools { 
        maven 'maven_3_9_11'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=quattrosec_buggywebapp -Dsonar.organization=quattrosec -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=a2561f56cd7ac220e56326be4f90bea599756566'
			}
        } 
  }
}
