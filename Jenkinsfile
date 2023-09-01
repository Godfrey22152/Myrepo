CODE_CHANGES = getGitChanges()
pipeline {
    agent any

    stages {
        stage('Build') {
          when {
            expression {
              BRANCH_NAME == 'main' && CODE_CHANGES == true
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
                echo 'Deployimg the Application'
            }
        }
    }
}
