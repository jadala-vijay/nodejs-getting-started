pipeline {
    agent any

    stages {
        stage('clone git'){
            steps {
            git https://github.com/jadala-vijay/nodejs-getting-started
            }
        }

        stage('install dep') {
            steps {
            sh 'npm istall'
            }
        }

        stage('run build') {
            steps {
            sh 'npm run build'
            }
        }
        stage('test stage') {
            steps {
            sh 'npm test'
            }
        }
    }
}
