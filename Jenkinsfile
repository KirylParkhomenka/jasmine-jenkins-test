pipeline {
    agent any

    stages {
        stage ('Build') {
            steps {
                sh 'export PATH=/usr/local/bin'
                sh 'npm --version'
                sh 'npm install'
            }
        }
        stage ('Test') {
            steps {
                sh 'node_modules/.bin/jasmine spec/jasmine_examples/PlayerSpec.js'
            }
        }
    }
}