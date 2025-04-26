pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/Chetan-Y-Patil/Pothole-Detection-Using-YOLO.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                script {
                    docker.build('pothole-app')
                }
            }
        }

        stage('Run Docker Container') {
            steps {
                script {
                    docker.image('pothole-app').run()
                }
            }
        }
    }
}
