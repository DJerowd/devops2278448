pipeline{

    agent any

    stages {
        stage('Build TADS') {
            steps {
                env.PATH = "${tool 'Nodejs'}/bin:${env.PATH}"
                sh '''
                        npm install
                '''
            }
        }
        stage('Test NPM') {
            steps {
                sh '''
                    npm test
                '''
            }
        }
        stage('Construindo Docker') {
            steps {
                sh '''
                    docker build .
                '''
            }
        }
        stage('Compose Docker') {
            steps {
                sh '''
                    docker compose up
                '''
            }
        }
    }
}