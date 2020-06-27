pipeline {
   agent any

   stages {
      stage('git clone') {
         steps {
            echo 'Cloning'
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
