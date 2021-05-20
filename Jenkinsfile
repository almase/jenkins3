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
                sh 'sudo apt update'
		sh 'sudo apt upgrade'
		sh 'sudo apt install sudo'
		sh 'sudo chown -R 987:980 "/.npm"'
                sh 'npm install ' 
            }
        }
    }
}

