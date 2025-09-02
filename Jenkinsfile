pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Make sure SCM uses the correct URL from Jenkins job configuration
                checkout scm
            }
        }
        stage('Build') {
            steps {
                sh 'echo Building Hello World app...'
            }
        }
        stage('Test') {
            steps {
                sh 'echo Running tests...'
            }
        }
        stage('Run') {
            steps {
                sh 'node app.js'
            }
        }
    }
}
