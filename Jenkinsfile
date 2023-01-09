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
               sh 'gradle -v'
                 sh 'echo $GRADLE_HOME'
                sh 'gradle build '
            }
        }
        
         
     }
 }
