pipeline {
    agent any
    stages {
        stage('git checkout') {
            steps {
                echo 'Checking out code..'
                // git branch: 'main',
                //     credentialsId: 'your-credentials-id',
                //     url: 'https://github.com/henrykrop2022/awscicd-week13-automation.git'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}