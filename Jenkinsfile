pipeline {
    agent none
    stages {
        stage('JS vulnerability check') {
            agent {
                docker 'gruebel/retirejs:latest'
                args '--entrypoint ""'
            }
            steps {
                sh 'retire'
            }
        }
    }
}

