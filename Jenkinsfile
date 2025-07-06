pipeline {
    agent any
    stages {
        stage('Clone') {
            steps {
               git url: 'https://github.com/TALSAGI1/tal_prod_ci_cd.git'
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
