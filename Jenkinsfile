pipeline {
  agent any
  tools { 
    maven 'Maven_3_8_4'  
  }
  stages {
    stage('CompileandRunSonarAnalysis') {
      steps {	
        sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=aasgbuggywebapp1994 -Dsonar.organization=asgbuggywebapp1994 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=9e80e8ffc4ff359e4ebf515997cb4b5297f145ab'
      }
    }
  }
}
