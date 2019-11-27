pipeline {
    agent { docker { image 'node:6.3' } }
    stages {
        stage('build') {
            steps {
                sh 'echo "Deploying now"'
                sh 'npm --version'
            }
        }
    }
}
