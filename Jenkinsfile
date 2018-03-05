pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
		sh 'git clone https://github.com/unixbhaskar/dockerjenkins.git docksjen5'
            }
        }
	
        stage('Test') {
            steps {
                echo 'Testing..'
		sh 'git log -1'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
		sh 'vmstat 1 1'
            }
        }
    }
}   
