pipeline {
    agent any

    stages {
        stage('Build TADS') {
            steps {
                sh 'npm install'
                sh 'npm test'
            }
        }
    }
}