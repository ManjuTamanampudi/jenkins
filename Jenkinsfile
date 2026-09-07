pipeline {
    agent {
                label 'ROBOSHOP'
    }
    stages {
        stage('build') {
            steps {
                 script {
                     echo "building the project..."
                 }
            }
        }
        stage('test') {
            steps {
                script {
                     echo "testing the project..."
                 }
            }
        }
        stage('deploy') {
            steps {
                script {
                     echo "deploying the project..."
                 }
            }
        }
    }
}