pipeline {
   agent any

   stages {
      stage('Build') {
         steps {
            // Get some code from a GitHub repository
            git branch: 'readme-branch', url: 'https://github.com/sefilang/helloworld.git'
            // print 
           echo 'start build'
            sh label: '', script: 'ls'
           sh label: '', script: 'cat sefi.txt'

         }

         post {
            success {
                echo 'success'
            }
         }
      }
   }
}
