// stage wise timestamp

pipeline {
    agent any
    
    stages {
        stage('Stage 1') {
            steps {
                    echo 'Running Stage 1...'
                }
            }
        }
        
        stage('Stage 2') {
            steps {
                timestamps {
                    echo 'Running Stage 2...'
                }
            }
        }
        
        stage('Stage 3') {
            steps {
                timestamps {
                    echo 'Running Stage 3...'
                }
            }
        }
        
        stage('Stage 4') {
            steps {
                timestamps {
                    echo 'Running Stage 4...'
                }
            }
        }
    }
