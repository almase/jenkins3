pipeline {
    agent {
        docker {
            image 'almase/ubuntu_jenkins:v1'' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'sudo apt-get update'
		sh 'sudo apt-get install nodejs'
		sh 'sudo chown -R 987:980 "/.npm"'
                sh 'npm install ' 
            }
        }
    }
}

