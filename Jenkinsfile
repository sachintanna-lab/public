pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                retry(3) {
                echo 'Building..'
                rehthetjety
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
