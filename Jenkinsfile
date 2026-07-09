pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Verify Website Files') {
            steps {
                bat 'dir'
            }
        }

        stage('Build Successful') {
            steps {
                echo 'Corporate Website Build Completed Successfully!'
            }
        }

    }

    post {
        success {
            echo 'Pipeline executed successfully.'
        }

        failure {
            echo 'Pipeline failed.'
        }
    }
}