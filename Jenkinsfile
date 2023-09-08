pipeline {
    agent {
        docker { image 'node:18.17.1-alpine3.18' }
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
