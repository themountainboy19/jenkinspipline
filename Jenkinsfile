pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                script {
                    docker.build('my-first-pipeline')
                }
            }
        }
        stage('Run Docker Container') {
            steps {
                script {
                    docker.image('my-first-pipeline').run('-d -p 8085:80')
                }
            }
        }
    }
}
