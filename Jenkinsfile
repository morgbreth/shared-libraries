pipeline {
    agent {
        label 'docker-agent'
    }
    stages {
        stage('Build') {
            steps {
                script {
                    // Your build steps here
                    sh 'docker build -t myapp .'
                }
            }
        }
        stage('Test') {
            steps {
                script {
                    // Your test steps here
                    sh 'docker run myapp test'
                }
            }
        }
    }
}
