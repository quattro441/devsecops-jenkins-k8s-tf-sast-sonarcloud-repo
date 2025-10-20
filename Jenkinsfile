pipeline {
  agent any
  tools { 
        maven 'maven_3_9_11'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=quattrosec_buggywebapp -Dsonar.organization=quattrosec -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=6b0defa2e7880e6b125cb848dfe9ff3917a5d1f0'
			}
        } 
  }
}
