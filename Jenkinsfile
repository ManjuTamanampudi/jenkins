pipeline {
    // agent {
    //             label 'ROBOSHOP'
    // }
    agent any
     environment {
        COURSE = "Jenkins"
    }
    options {
        disableConcurrentBuilds()
        timeout(time: 5, unit: 'MINUTES')
    }
    stages {
        stage('build') {
            steps {
                 script {
                     echo "building the project..."
                     exit 1
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
    // post build
    post { 
        always { 
            echo 'I will always say Hello again!'
        }
        success {
            echo "pipeline success"
        }
        failure {
            echo "pipeline failure"
        }
    }
}