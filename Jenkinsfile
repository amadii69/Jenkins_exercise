pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                // Pull code from GitHub
                checkout scm
            }
        }

        stage('Run Test Script') {
            steps {
                sh '''
                  echo "Running test.sh in Jenkins workspace"
                  ls -l
                  ./test.sh
                '''
            }
        }
    }
}