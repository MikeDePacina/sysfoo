pipeline{
    agent any
    tools {
        maven 'Maven 3.9.9'
    }
    stages{
        stage('build'){
            sh 'mvn compile'
        }

        stage('test'){
            sh 'mvn clean test'
        }

        stage('package'){
            sh 'mvn package -D skipTests'
        }
    }
}