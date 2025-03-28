/* Requires the Docker Pipeline plugin */
pipeline {
    agent {
        docker {
            image 'node:22.14.0-alpine3.21'
            args '-v /var/run/docker.sock:/var/run/docker.sock' // Only if you need Docker-in-Docker
        }
    }
    stages {
        stage('build') {
            steps {
                sh 'node --version'
            }
        }
    }
}
