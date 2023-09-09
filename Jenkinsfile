pipeline {
    agent any
    stages {
        stage('Docker Build and Run') {
            steps {
                script {
                    def workspacePath = pwd()
                    // Print the workspace path
                    echo "Workspace Path: $workspacePath"
                    
                    // Convert the workspace path to a valid Windows-style absolute path
                    def windowsStylePath = powershell(returnStatus: true, script: "Resolve-Path -Path \"$workspacePath\"")

                    // Print the resolved path
                    echo "Resolved Path: $windowsStylePath"

                    // Use windowsStylePath as the working directory
                    docker.image('nginx:alpine').inside("-w $windowsStylePath") {
                        // Your Docker build and run steps here
                    }
                }
            }
        }
    }
}
