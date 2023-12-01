pipeline {
    agent any
    tools {
        Nodejs '21.3.0'
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