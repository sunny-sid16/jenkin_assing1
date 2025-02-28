pipeline {
    agent any
    triggers {
        pollSCM('* * * * *')  // Check every minute (or use webhook)
    }
    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/sunny-sid16/jenkin_assing1.git', branch: 'develop'
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
