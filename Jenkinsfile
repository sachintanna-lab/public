pipeline {
    agent any
    
    environment {
        DISABLE_AUTH = credentials('jenkins_credentials')
        DB_ENGINE    = 'sqlite'
    }

    stages {
        stage('Build') {
            steps {
                echo 'I am being read'
                echo "Environment variable read: ${DISABLE_AUTH}"
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
     post {
        always {
            echo 'This will always run'
        }
        success {
            echo 'This will run only if successful'
            mail to: 'Sachin.Tanna@ibm.com',
             subject: "Success",
             body: "Congratulations, you now know how to send emails from Jenkins"
        }
        failure {
            echo 'This will run only if failed'
        }
        unstable {
            echo 'This will run only if the run was marked as unstable'
        }
        changed {
            echo 'This will run only if the state of the Pipeline has changed'
            echo 'For example, if the Pipeline was previously failing but is now successful'
        }
    }
}
