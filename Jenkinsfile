pipeline {
    agent any
    options{
        skipdefaultcheckout(true)
    }
    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main', url: 'https://github.com/adil-learning/Jenkins-learning'
            }
        }
        stage('Build') {
            steps {
                sh 'echo "Build the code"'
            }
        }
        stage('Test the code') {
            steps {
                sh 'echo "testing the code to the test environment"'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo "Deploying the code to check the functionality before release into the production"'
            }
        }
    }
    post{
    success{
        bat 'echo "build is successful"'
    }
    failure{
        bat 'echo "build failed"'
    }
}
}

