pipeline {
    agent any

    environment {
        BRANCH_NAME = 'main'
        GIT_URL = 'https://github.com/henrykrop2022/awscicd-week13-automation.git'
    }
    stages {
        stage('git checkout') {
            steps {        
                git branch: "${BRANCH_NAME}", url: "${GIT_URL}"
                }
        }
        stage('docker build') {
            steps {
                sh 'docker build -t henrykrop2022/awscicd-week13-automation .'
                sh 'docker images'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}