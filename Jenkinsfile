pipeline {
    agent {
        docker {
            image 'nginx:alpine'
            args +pwd()
        }
    }
    stages {
        stage('Build') {
            steps {
                echo "Success"
            }
        }
    }
}
