pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
		sh 'ls -lath'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
		sh 'uname -a'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
		sh 'who -r'
            }
        }
    }
}

