pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
            }
        }
        stage('Test') {
            steps {
                echo 'Running unit tests...'
                sh 'pytest tests/'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                sh 'bash scripts/deploy.sh'
            }
        }
    }
}
