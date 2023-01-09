pipeline {
     agent { 
     docker {
      image 'gradle:7-jdk11'
    }
     }
     stages {
         
        stage('Clone Project') {
             steps {                  
                  checkout scm                  
             }
         }
        
        stage('Build') {
            steps {
              
                sh 'gradle build '
            }
        }
        
         
     }
 }
