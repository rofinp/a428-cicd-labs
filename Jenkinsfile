pipeline {
    agent {
        docker {
            image 'node:lts-bookworm-slim'
            args '-p 3000:3000'
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'npm cache clean --force'
                sh 'npm install'
            }
        }
    }
}
