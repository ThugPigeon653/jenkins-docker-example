pipeline {
    agent {
        docker {
            image 'nginx:alpine'
            args 'w'+args '-w C:\\Users\\LNeil\\Documents\\Programming\\jenkins-destination'
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
