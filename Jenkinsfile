pipeline {
    agent {
        docker {
            image 'nginx:alpine'
            args 'w'+pwd()
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
