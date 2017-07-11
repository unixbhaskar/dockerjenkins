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
		sh '/home/bhaskar/AdmScripts/kernel_module_list.sh'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
		sh '/home/bhaskar/AdmScripts/osstat'
            }
        }
    }
}
