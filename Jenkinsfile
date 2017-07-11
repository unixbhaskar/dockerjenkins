pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
		sh '/home/bhaskar/AdmScripts/disk_usage_monitor.sh'
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
