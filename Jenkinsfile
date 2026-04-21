pipeline {
    agent any

    stages {
        stage('Clone Code') {
            steps {
                git 'https://github.com/AyushSirohi/traineeTesting.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                script {
                    docker.build("my-app-image")
                }
            }
        }
    }
}
