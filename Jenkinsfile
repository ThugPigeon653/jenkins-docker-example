pipeline {
    agent any

    stages {
        stage('Build and Run Windows Docker Container') {
            steps {
                script {
                    // Build and run the Windows Docker container
                    bat 'docker run --rm mcr.microsoft.com/windows/nanoserver:1909 echo Hello, Windows!'
                }
            }
        }
    }
}
