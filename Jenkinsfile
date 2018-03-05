pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..Running ${env.BUILD_ID} on ${env.JENKINS_URL}'
		sh 'git clone https://github.com/unixbhaskar/dockerjenkins.git docksjen12'
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
		sh 'vmstat 1 1'
            }
        }

      post {
        success {
            echo 'Build succeeded.'
        }
        unstable {
            echo 'This build returned an unstable status.'
        }
        failure {
            echo 'This build has failed. See logs for details.'
        }
      }
  }
}
   
