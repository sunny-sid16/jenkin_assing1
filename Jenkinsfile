pipeline {
    agent any
    triggers {
        pollSCM('* * * * *')  // Check every minute (or use webhook)
    }
    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/your-username/your-repo.git', branch: 'develop'
            }
        }
        stage('Build') {
            steps {
                echo 'Building the application...'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }
    }
}
