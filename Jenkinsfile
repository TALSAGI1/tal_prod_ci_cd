pipeline {
    agent any
    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/your-username/ci-cd-project.git'
            }
        }
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
