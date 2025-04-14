pipeline {
    agent any
    stages {
        stage('clone code') {
            steps {
                checkout scm
            }
        }
        stage('installing dependencies') {
            steps {
                sh 'npm install'
            }
        }
        stage('running app locally') {
            steps {
                sh 'node app.js'
            }
        }
    }
}