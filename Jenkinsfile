pipeline {
    agent any

    stages {
        stage('Build') {
            agent {
                docker { image 'maven:3.9.9-eclipse-temurin-21-alpine' }
            }
            steps {
                echo 'Building..'
                sh "ls -la ${pwd()}"
                sh 'mvn --version'            
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
