pipeline {
     agent { 
     docker {
      image 'gradle:7-jdk11'
       args '-v /home/cloud_user/jenkins:/var/jenkins_home'
    }
     }
     stages {
         
        stage('Clone Project') {
             steps {                  
                  checkout scm                  
             }
         }
        
        stage('listing1') {
             steps {                  
                    
                  sh 'ls -l'
             }              
         }
        
        stage('Build') {
            steps {
               
                sh './gradle wrapper '
            }
        }
        
         
     }
 }
