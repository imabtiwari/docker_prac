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
            sh 'docker build -t "specular-Shwetank" .'
         }
         
      }
      stage('docker push to registery') {
         steps {
            echo 'docker push imabtiwari/repo'
         }
         
      }
   }
}
