pipeline {
    agent any
    environment { DEPLOY_TO = 'qa'}
    stages {
        stage('Stage1') {
            when {
              environment name: 'DEPLOY_TO', value: 'qa'
            }
            steps {
              echo 'Running Stage1 for QA'
            }
        }
       stage('Stage2') {
            when {
              environment name: 'DEPLOY_TO', value: 'production'
            }
            steps {
              echo 'Running Stage2 for production'
            }
        }
    }
}