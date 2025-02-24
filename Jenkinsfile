pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/BestBoss7/myproject.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
            }
        }
    }
}

