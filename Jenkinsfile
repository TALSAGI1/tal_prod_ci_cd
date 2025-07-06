pipeline {
    agent any
    stages {
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t myapp .'
            }
        }
        stage('Run Container Locally') {
            steps {
                sh 'docker run -d -p 5000:5000 myapp'
            }
        }
    }
}
