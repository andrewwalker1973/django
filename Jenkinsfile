#!groovy
pipeline {
    agent {
        docker { image 'hysnsec/safety:latest' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'ls -l'
            }
        }
    }
}
