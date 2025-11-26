pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing...'
            }
        }

        stage('Deploy') {
            when { success() }   // run only if Test succeeds
            steps {
                echo 'Deploying...'
            }
        }
    }
}
