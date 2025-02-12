pipeline {
    agent any

    environment {
        BRANCH_NAME = 'main'
        GIT_URL = 'https://github.com/henrykrop2022/awscicd-week13-automation.git'
        IMAGE_TAG = 'henrykrop2022/awscicd-week13-automation'
        IMAGE_VERSION = "${BUILD_NUMBER}"
    }
    stages {
        stage('git checkout') {
            steps {        
                git branch: "${BRANCH_NAME}", url: "${GIT_URL}"
                }
        }
        stage('docker build') {
            steps {
                sh 'docker build -t "${IMAGE_TAG}:${IMAGE_VERSION}" .'
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