pipeline {
    agent any

    parameters {
        string(name: 'BRANCH', defaultValue: 'master', description: 'Which branch to build?')
        choice(name: 'ENVIRONMENT', choices: ['Development', 'Staging', 'Production'], description: 'Choose an environment.')
        booleanParam(name: 'NOTIFY', defaultValue: true, description: 'Send notifications?')
    }

    stages {
        stage('Display') {
            steps {
                echo "Building branch: ${params.BRANCH}"
                echo "Deploying to: ${params.ENVIRONMENT}"

                script {
                    if (params.NOTIFY) {
                        echo 'Notifications are ON'
                        // Add steps to send notifications here.
                    } else {
                        echo 'Notifications are OFF'
                    }
                }
            }
        }
    }
}
