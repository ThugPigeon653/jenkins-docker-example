pipeline {
    agent {
        docker {
            image 'nginx:alpine'
            dir '/workspace'
        }
    }
    stages {
        stage('Build') {
            steps {
                echo 'Success'
            }
        }
    }
}
