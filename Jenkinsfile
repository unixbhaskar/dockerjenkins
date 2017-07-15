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
		sh 'ipcs'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
		sh 'vmstat 1 1'
            }
        }
    }
    post {
        always {
	    mail to : 'unixbhaskar@gmail.com',
                 subject : "Checking post hook",
		   body  : "heck"
   }	   
 }  
}
