pipeline {
    agent {
        docker {
            image 'node:6-alpine'
            args '-p 9000:9000'
        }
    }
    environment {
        CI = 'true' 
    }
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        stage('Test') { 
            steps {
                echo "OK done"
            }
        }
    }
}