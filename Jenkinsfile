#!groovy
pipeline {
    agent {
        docker { image 'hysnsec/safety:latest'
               args '--entrypoint='
               }
    }
    stages {
        stage('Test') {
            steps {
                sh 'cd django'
                sh 'safety check -r requirements.txt '
        }
    }
}
}
