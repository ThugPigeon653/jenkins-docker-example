pipeline {
    agent any

    stages {
        stage('Build and Run') {
            steps {
                script {
                    // Build the Docker image
                    def dockerImage = docker.build('my-web-app:latest')

                    // Run the Docker container with the appropriate port mapping
                    def dockerContainer = dockerImage.run('-p 80:80 -d')

                    // Show container logs for troubleshooting
                    echo dockerContainer.logs().stdout
                }
            }
        }
    }
}