pipeline {
    agent none
    stages {
        stage('test') {
            agent {
                docker {
                    { image 'hadolint/hadolint:latest-alpine' }
                }
            }
            steps {
                hadolint Dockerfile
            }
        }
    }
}