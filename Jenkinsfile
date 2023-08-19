@Library('jenkins-ci-cd-library') _

pipeline {
    agent any
    parameters {
        string(name: 'VALUE_A', defaultValue: '5', description: 'First value')
        string(name: 'VALUE_B', defaultValue: '7', description: 'Second value')
    }
    stages {
        stage('Addition Stage') {
            steps {
                add("${params.VALUE_A}", "${params.VALUE_B}")
            }
        }
    }
}
