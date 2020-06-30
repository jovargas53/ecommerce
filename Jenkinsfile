pipeline {
    agent {
        docker {
             image 'node:10-alpine' 
                    }
    }
    stages {
	
	stage('Version NPM') { 
            steps {
                sh 'npm -version' 
				  }
        }
		
	stage('Checkout ProyectoNPM') {
        steps {
            git branch: 'master',
                url: 'https://github.com/diro7/ecommerce.git'

            sh "ls -lat"
			}
		}
		
	stage('Build') { 
            steps {
                sh 'npm install' 
				  }
        }
	
    }
}
