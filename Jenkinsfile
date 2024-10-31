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
                sh 'cd django'
                sh 'pwd'
                sh 'npm install'
                sh 'npm install retire'
                sh './node_modules/retire --outputformat json --outputpath retirejs-report.json'
        }
    }
}
}
