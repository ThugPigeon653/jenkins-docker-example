pipeline {
    agent {
        docker { image 'nginx:alpine' }
    }
    stages {
        stage('Build') {
            steps {
                script {
                    def workspacePath = pwd() // Get the workspace path
                    echo "Workspace path: ${workspacePath}"
                }
            }
        }
    }
}
