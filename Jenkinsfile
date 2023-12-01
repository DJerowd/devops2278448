pipeline {
    agent any
    tools {
        node.js '21.3.0'
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