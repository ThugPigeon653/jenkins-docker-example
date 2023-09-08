
pipeline {
    agent {
        docker {
            image 'nginx:alpine'
            args '-w c://users/lneil/documents/programming/jenkins-destination'
        }
        docker { image 'nginx:alpine' }
    }
