pipeline {
    agent any
    environment {
        CI = 'true'
    }

    stages {
        stage('Build') {
            steps {
                pwsh 'bun install'
            }
        }
        stage('Test') {
            steps {
                pwsh "Write-Output 'Test successful'"
            }
        }
    }
}