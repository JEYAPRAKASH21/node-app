pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/JEYAPRAKASH21/node-app.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                script {
                    docker.build("node-app")
                }
            }
        }
    }
}
