pipeline{

    agent any

    stages {
        stage{"Build TADS"} {
            steps {
                sh 'docker --version'
                sh 'docker-compose -v'
                sh 'java -version'
            }
        }
    }
}