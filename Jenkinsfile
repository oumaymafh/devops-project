pipeline {
    agent any

    stages {
        stage('Clone repository') {
            steps {
                git 'https://github.com/oumayma/devops-project.git'
            }
        }
        stage('Build') {
            steps {
                sh './mvnw clean install'
            }
        }
        stage('Test') {
            steps {
                sh './mvnw test'
            }
        }
    }
}