#!/usr/bin/env groovy

pipeline {

    agent {
        docker {
            image 'python:slim'
            args '-u root'
        }
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'python3 testy.py'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                sh 'python3 testy.py'
            }
        }
    }
}
