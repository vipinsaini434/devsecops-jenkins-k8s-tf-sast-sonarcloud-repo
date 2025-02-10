pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=secchampquantum -Dsonar.organization=secchampquantum -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=f07f947407c6f291d49a3095f1b31157632bb5e4'
			}
        } 
  }
}
