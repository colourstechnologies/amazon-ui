pipeline {
    agent any
    
    options {
        timestamps()  // This enables timestamps for the entire pipeline
    }
    
    stages {
        stage('Stage 1') {
            steps {
                echo 'Running Stage 1...'
                sleep(time: 4, unit: 'SECONDS')
            }
        }
        
        stage('Parallel Stages') {
            parallel {
                stage('Stage 2') {
                    steps {
                        echo 'Running Stage 2...'
                        sleep(time: 4, unit: 'SECONDS')
                    }
                }
                
                stage('Stage 3') {
                    steps {
                        echo 'Running Stage 3...'
                        sleep(time: 4, unit: 'SECONDS')
                    }
                }
            }
        }
        
        stage('Stage 4') {
            steps {
                echo 'Running Stage 4...'
                sleep(time: 4, unit: 'SECONDS')
            }
        }
    }
}
