
pipeline {
    agent {
        docker { image 'nginx:alpine',  args '-w /workspace' }
    }
    stages {
        stage('Build') {
            steps {
                echo "Success"
            }
        }
    }
}
