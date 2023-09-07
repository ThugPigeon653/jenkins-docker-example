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

                    // Sleep to keep the Jenkins agent running (you can also use other methods)
                    sleep(time: 60, unit: 'SECONDS')

                    // Stop and remove the Docker container
                    dockerContainer.stop()
                    dockerContainer.remove()
                }
            }
        }
    }
}
