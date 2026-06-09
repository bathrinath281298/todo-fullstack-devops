pipeline {
    agent any

    stages {

        stage('Git Check') {
            steps {
                bat 'git --version'
            }
        }

        stage('Docker Check') {
            steps {
                bat 'docker --version'
            }
        }

        stage('Docker Compose Check') {
            steps {
                bat 'docker compose version'
            }
        }
    }
}	