pipeline {
   agent any

   stages {
      stage('git fetching directories') {
         steps {
            sh 'ls -la'
            sh 'pwd'
         }
         
      }
      stage('Docker Bulid') {
         steps {
            sh 'docker build -t "imabitiwari/jenkins-1" .'
         }
         
      }
      stage('docker push to registery') {
         steps {
            sh 'echo "abhishek@51" | docker login --username imabtiwari --password-stdin'
            sh 'docker push imabitiwari/jenkins-1:1'
         }
         
      }
   }
}
