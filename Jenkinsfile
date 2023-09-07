pipeline {
    agent any
    
    stages {
        stage('Build and Push Docker Image') {
            steps {
                script {
                    def dockerImage = docker.build('myapp:latest')
                    dockerImage.push()
                }
            }
        }
    }
}
