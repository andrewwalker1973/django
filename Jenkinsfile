#!groovy
pipeline {
    agent {
        docker { image 'node:alpine3.10'
               args '--entrypoint='
               }
    }
    stages {
        stage('Test') {
            steps {
                sh 'id'
                sh 'cd django'
                sh 'npm install'
                sh 'npm install -g retire'
                sh 'retire --outputformat json --outputpath retirejs-report.json'
        }
    }
}
}
