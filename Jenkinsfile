pipeline {
    agent any
    stages {
        stage('git checkout') {
            steps {
                git 'https://github.com/henrykrop2022/awscicd-week13-automation.git'
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