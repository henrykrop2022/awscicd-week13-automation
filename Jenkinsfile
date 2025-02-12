pipeline {
    agent any
    stages {
        stage('git checkout') {
            steps {
                git ''
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