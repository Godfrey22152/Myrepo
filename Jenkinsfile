pipeline {
    agent any

    stages {
        stage('Build') {
            when {
                expression {
                    changesetExists()
                }
            }
            steps {
                echo 'Building the Application'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing the Application'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the Application'
            }
        }
    }
}
