pipeline {
    agent any
    stages {
        stage('Docker Build and Run') {
            steps {
                script {
                    def workspacePath = pwd()
                    // Use workspacePath as the absolute working directory
                    docker.image('nginx:alpine').inside("-w $workspacePath") {}
                }
            }
        }
    }
}
