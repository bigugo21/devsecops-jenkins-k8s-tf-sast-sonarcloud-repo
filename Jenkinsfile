pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=ugosecurityguru -Dsonar.organization=ugosecurityguru -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=a143338f8e7c9ed0c14ef033953f4ec187d447d9'
			}
        } 
  }
}
