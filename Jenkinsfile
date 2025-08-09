pipeline{
    agent any
    stages{
        stage('checkout code'){
        steps{
            git 'https://github.com/adil-learning/Jenkins-learning'
        }
        }
        stage('Build'){
            steps{
                sh 'echo "Build the code"'
            }
        }
        stage('Test the code'){
            steps{
                sh 'echo "testing the code in the test environment"'
            }
        }
        stage('Deploy'){
            steps{
                sh 'echo "Deploying the code to check the functionality before release into the production"'
            }
        }
    }
}
