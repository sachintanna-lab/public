pipeline {
    agent { docker { image 'maven:3.3.3' } }
    stages {
        stage('build') {
            steps {
                sh 'echo "Deploying now"'
                sh 'mvn --version'
            }
        }
    }
}
