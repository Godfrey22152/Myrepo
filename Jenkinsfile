pipeline {
    agent any

    stages {
        stage('Build') {
            when {
                expression {
                    BRANCH_NAME == 'main' && changesetExists()
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
