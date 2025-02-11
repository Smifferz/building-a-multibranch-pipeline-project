pipeline {
    agent any
    environment {
        CI = 'true'
    }

    stages {
        stage('Build') {
            steps {
                sh 'bun install'
            }
        }
        stage('Test') {
            steps {
                sh './jenkins/scripts/test.sh'
            }
        }
    }
}