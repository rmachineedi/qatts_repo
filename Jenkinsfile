pipeline {
    agent any

    stages {
        stage('git_clone') {
            steps {
                git branch: 'main', url: 'https://github.com/rmachineedi/qatts_repo.git'
            }
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'docker-compose -f qatts3.yml up -d'
            }
        }
    }
}
