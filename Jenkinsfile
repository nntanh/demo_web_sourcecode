pipeline {
    // agent any
    agent {
        docker {image 'node:19.6.0'} //eviroment
    }

    stages {
        stage('build code') {
            steps {
                sh '''
                npm install
                npm run build                
                '''
            }            
        }
        stage ('test') {
            steps {
                sh 'npm run test'
            }
        }
    }
}
