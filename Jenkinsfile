pipeline {
    agent any 
    stages {
        stage('check cmd') {
            steps {
                sh 'docker-compose version'
            }
        }
        stage('build') {
            steps {
                sh 'docker-compose up -d'
                sh 'docker exec nginx curl http://localhost'
            }
        }
    }
}
