#!groovy
pipeline {
    agent none
   stages {   
    stage('Maven Install') {
    agent {         
       docker {          
         image 'hysnsec/safety'         
     }       
  }       
  steps {
       sh 'safety check'
       }
     }
   }
 }
