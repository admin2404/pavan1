pipeline {
 agent any
  stages {
      stage('Pull') {
         steps {
             git 'https://github.com/admin2404/pavan1.git'
         }
      }
      stage('Compile') {
         steps {
            bat 'mvn compile'
         }
      }
	   stage('Test') {
         steps {
            bat 'mvn test'
         }
      }
	   stage('Package') {
         steps {
            bat 'mvn package'
         }
      }
      stage('Execute') {
         steps {
            bat 'java -jar "C:/Windows/System32/config/systemprofile/AppData/Local/Jenkins/.jenkins/workspace/cts_pip/target/ctsproj1-1.0-SNAPSHOT.jar"'
         }
      }
   }
}
