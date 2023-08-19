pipeline {
    agent any
    
    stages {
        stage('Stage 1') {
            steps {
                echo 'Running Stage 1...'
            }
        }
        
        stage('Stage 2') {
            steps {
                echo 'Running Stage 2...'
                script {
                    try {
                        sh 'this-command-does-not-exist' // Intentional error
                    } catch (Exception e) {
                        echo "An error occurred: ${e.getMessage()}"
                    }
                }
            }
        }
        
        stage('Stage 3') {
            steps {
                echo 'Running Stage 3...'
            }
        }
        
        stage('Stage 4') {
            steps {
                echo 'Running Stage 4...'
            }
        }
    }
}

