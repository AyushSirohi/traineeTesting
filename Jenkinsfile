pipeline {
    agent any

    stages {
        stage('Clone Code') {
            steps {
                git branch: 'main', url: 'https://github.com/AyushSirohi/traineeTesting.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                dir('Assignment 10 Trainee testing') {
                    script {
                        docker.build("my-app-image")
                    }
                }
            }
        }
    }
}
