// Build Timestamp Plugin

pipeline {
    agent any 

    options {
        timestamps()  // This enables timestamps for the entire pipeline
    }

    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out code...'
                // Add your SCM checkout steps here if needed.
                sleep(time: 4, unit: 'SECONDS')
            }
        }

        stage('Build') {
            steps {
                echo 'Building...'
                // Add your build steps here.
                sleep(time: 4, unit: 'SECONDS')
            }
        }

        stage('Test') {
            steps {
                echo 'Testing...'
                // Add your test steps here.
                sleep(time: 4, unit: 'SECONDS')
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Add your deployment steps here.
                sleep(time: 4, unit: 'SECONDS')
            }
        }

    }
}
