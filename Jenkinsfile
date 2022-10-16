
pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
      stages {
        stage('Checkout GIT') {
            steps {
                echo 'Pulling...';
                git branch: 'main',
                url : 'https://github.com/ChamesBenRezigueEsprit/Devops-Back.git'
            }
        }
        stages {
        stage('Testing maven') {
            steps {
                sh """mvn -version"""
            }
        }
    }
}
