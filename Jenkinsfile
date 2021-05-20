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
                sh 'apt updte'
		sh 'apt upgrade'
		sh 'apt install sudo'
		sh 'udo chown -R 987:980 "/.npm"'
                sh 'npm install ' 
            }
        }
    }
}

