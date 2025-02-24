pipeline {
    agent any
    tools {
        maven 'Maven' 
    }
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/BestBoss7/myproject.git'
            }
        }
        stage('Build') {
            steps {
                bat 'mvn clean package' 
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }
    }
}
