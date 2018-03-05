pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..Running ${env.BUILD_ID} on ${env.JENKINS_URL}'
		sh 'git clone https://github.com/unixbhaskar/dockerjenkins.git docksjen20'
            }
        }
	
        stage('Test') {
            steps {
                echo 'Testing.. Running ${env.BUILD_ID} on ${env.JENKINS_URL}'
		sh 'git log -1'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....Running ${env.BUILD_ID} on ${env.JENKINS_URL}'
		sh '/home/bhaskar/AdmScripts/version-check.sh'
            }
        }

  }
}
   
