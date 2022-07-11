pipeline {
    agent any

    stages {
        stage('git_clone') {
            steps {
                git branch: 'main', url: 'https://github.com/rmachineedi/qatts_repo.git'
            }
        }
        stage('build') {
            steps {
                bat 'docker-compose -f qatts3.yml up --force-recreate -d'
            }
        }
    } 
}
