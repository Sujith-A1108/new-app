pipeline {
    agent any
    tools {
        maven 'Maven3'
        jdk 'JDK17'
    }
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Sujith-A1108/new-app.git'
            }
        }
        stage('Build') {
            steps {
                bat 'mvn clean compile'
            }
        }
        stage('Test') {
            steps {
                bat 'mvn test'
            }
        }
        stage('Package') {
            steps {
                bat 'mvn package'
            }
        }
    }
}