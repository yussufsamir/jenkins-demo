pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/<your-username>/jenkins-demo.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building project...'
                sh 'python3 hello.py'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'pytest test_hello.py'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deployment simulated!'
            }
        }
    }
}
