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

        stage('Build Images') {
            steps {
                bat 'docker compose build'
            }
        }

        stage('Run Containers') {
            steps {
                bat 'docker compose up -d'
            }
        }

        stage('Verify Containers') {
            steps {
                bat 'docker ps'
            }
        }
    }
}