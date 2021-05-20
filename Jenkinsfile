pipeline {
    agent {
        docker {
            image 'node:14-buster' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
		sh 'npm  cache clean --force'
                sh 'npm install cowsay@1.2.0' 
            }
        }
    }
}

