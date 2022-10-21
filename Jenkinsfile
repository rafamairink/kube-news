pipeline {
    agent any
    
    stages {

        stages ('Build Docker Image') {
            steps {
                script {
                    dockerapp = docker.build("mairink/kube-news:${env.BUILD_ID}", '-f .src/Dockerfile ./src')
                }

            }

        }

    }

}
