pipeline {
    agent {
        docker { image 'node:22.11.0-alpine3.20' }
    }
    stages {
        stage('Test') {
            steps {
                sh '`id`'
                sh 'node --version'
                sh 'npm install -g retire'
                sh 'retire --path `pwd` --outputformat json --outputpath /{JENKINS HOME DIRECTORY}/reports/retirejs-report --exitwith 0'
                }
        }
    }
}
