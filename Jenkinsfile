
pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Checkout GIT') {
            steps {
                echo 'Pulling...';
                git branch: 'main',
                url : 'https://github.com/ChamesBenRezigueEsprit/Devops-Back.git'
            }
        }
        stage('Testing maven') {
            steps {
                sh """mvn -version"""
            }
        }
    }
}
