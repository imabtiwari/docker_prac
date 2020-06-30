pipeline {
   agent any
   
       environment {
        USER_NAME = 'imabtiwari'
        MY_PASSWORD = 'abhishek@51'
    }

   stages {
      stage('git fetching directories') {
         steps {
            sh 'ls -la'
            sh 'pwd'
         }
         
      }
      stage('Docker Bulid') {
         steps {
            sh 'docker build -t "imabtiwari/jenkins-1" .'
         }
         
      }
      stage('docker push to registery') {
         steps {
            sh 'echo ${MY_PASSWORD} | docker login --username ${USER_NAME} --password-stdin'
            sh 'docker push imabtiwari/jenkins-1:latest'
         }
         
      }
   }
}
