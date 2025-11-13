pipeline {
    agent any

    stages {
        stage('Build & Run') {
            steps {
                checkout scm
                sh 'docker build -t hello-app .'
                sh 'docker run --rm hello-app'
            }
        }
    }
}
