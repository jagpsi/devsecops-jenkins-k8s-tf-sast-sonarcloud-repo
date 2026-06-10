pipeline {
  agent any
  tools { 
        maven 'Maven_3_8_4'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=jagpsi -Dsonar.organization=jagpsi -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=5e3f77bafff78138c2427798e42b4c1232da9502'
			}
        } 
  }
}
