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
       sh 'docker run --rm -v ${PWD}:/src hysnsec/safety check'
       }
     }
   }
 }
