pipeline {
    agent any

    stages {
        stage('clone git'){
            steps {
            git  branch: 'main' , url: 'https://github.com/jadala-vijay/nodejs-getting-started.git'
            }
        }

        stage('install dep') {
            steps {
            sh 'npm install'
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
