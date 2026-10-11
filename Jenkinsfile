pipeline {
    agent { label 'dynamic-agent' }
    stages {
        stage('Verify') {
            steps {
                sh 'hostname'
                sh 'ls -R'
                sh 'cat css/style.css'
            }
        }
        stage('Run') {
            steps {
                sh 'node backend/server.js'
            }
        }
    }
}
