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
            sh 'sudo docker build -t "specular-shwetank" .'
         }
         
      }
      stage('docker push to registery') {
         steps {
            echo 'docker push imabtiwari/repo'
         }
         
      }
   }
}
