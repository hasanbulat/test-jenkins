pipeline {
    agent any 
    stages {
        stage('build') {
            steps {
                sh 'docker-compose up -d'
                sh 'docker exec nginx curl http://localhost'
            }
        }
    }
}
