pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Building application...'
            }
        }

        stage('Parallel Tests') {
            parallel {

                stage('Unit Test') {
                    steps {
                        echo 'Running unit tests...'
                        sh 'sleep 10'
                    }
                }

                stage('Security Scan') {
                    steps {
                        echo 'Running security scan...'
                        sh 'sleep 10'
                    }
                }
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }
    }
}