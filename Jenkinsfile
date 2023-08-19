pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo "Building the application"
            }
        }

        stage('Test') {
            steps {
                echo "Running tests"
                // Uncommenting the line below will make the build fail.
                sh "exit 1"
            }
        }
    }

    post {
        always {
            echo "This will always run, regardless of build status."
        }
        success {
            echo "Build was a success!"
        }
        failure {
            echo "Build failed!"
        }
    }
}
