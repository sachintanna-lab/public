pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                timeout(time: 3, unit: 'MINUTES') {
                echo 'Building..'
                }
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
