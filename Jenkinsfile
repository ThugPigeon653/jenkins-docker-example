pipeline {
    agent {
        docker {
            image 'nginx:alpine'
            args '-w c://users/lneil/documents/programming/jenkinsi-destination' // Pass the workspace as an environment variable
        }
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
