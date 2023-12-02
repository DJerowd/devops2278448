pipeline{

    agent any
    tools {
        nodejs 'Nodejs'
        docker 'Docker'
    }

    stages {
        stage('npm Install') {
            steps {
                
                sh '''
                        npm install
                '''
            }
        }
        stage('npm Test') {
            steps {
                sh '''
                    npm test
                '''
            }
        }
        stage('Docker build') {
            steps {
                sh '''
                    docker build .
                '''
            }
        }
        stage('Docker Compose') {
            steps {
                sh '''
                    docker compose up
                '''
            }
        }
    }
}