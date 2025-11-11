pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/your-org/your-repo.git'
            }
        }
        stage('Build') {
            steps {
                sh 'echo "Build step"'
            }
        }
        stage('Deploy') {
            steps {
                sh './scripts/deploy.sh staging'
            }
        }
    }
}
