pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Building the application...'
                sh 'docker build -t cloud-cicd-lab .'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing the application...'
                sh 'python3 --version'
            }
        }
    }
}
