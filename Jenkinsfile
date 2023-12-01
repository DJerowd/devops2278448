pipeline {
    agent any
    tools {
        nodejs '21.3.0'
    }

    stages {
        stage('Build TADS') {
            steps {
                sh 'npm install'
                sh 'npm test'
            }
        }
    }
}