
pipeline {
    agent any

    stages {
        stage('Build and Run') {
            steps {
                script {
                    def dockerImage = docker.build('my-web-app:latest')

                    def dockerContainer = dockerImage.run('-p 80:80 -d')
                }
            }
        }
    }
}