pipeline {
    agent any
    stages {
        stage('List and Count Files') {
            steps {
                sh 'ls -la'
                sh 'ls | wc -l'
            }
        }
        stage('Print Current User') {
            steps {
                sh 'whoami'
            }
        }
        stage('Create and Navigate Directory') {
            steps {
                sh 'mkdir myfolder'
                sh 'cd myfolder'
            }
        }
        stage('Create and Write to File') {
            steps {
                sh 'echo "Hello, Jenkins!" > mytextfile.txt'
            }
        }
        stage('Append to File') {
            steps {
                sh 'echo "Appending more content." >> mytextfile.txt'
            }
        }
        stage('Display File Content') {
            steps {
                sh 'cat mytextfile.txt'
            }
        }
        stage('Find and Replace') {
            steps {
                sh 'sed -i "s/Jenkins/CI-CD/g" mytextfile.txt'
                sh 'cat mytextfile.txt'
            }
        }
        stage('Compress and Archive Files') {
            steps {
                sh 'tar -czvf archive.tar.gz myfolder'
            }
        }
                stage('Compress and Archive Files') {
            steps {
                sh 'rm -rf myfolder'
            }
        }
    }
}
