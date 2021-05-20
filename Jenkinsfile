pipeline {
    agent {
        docker {
            image 'node:lts-buster-slim' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sudo chown -R 987:980 "/.npm"
                sh 'npm install' 
            }
        }
    }
}

