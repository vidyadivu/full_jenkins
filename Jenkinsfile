pipeline {
    agent any
    stages{
        stage('stage1'){
            steps{sh 'sleep 10'}
        }
        stage('stage2'){
            steps{sh 'sleep 10'}
        }
        stage('stage3'){
            parallel{
                stage('parallel 1'){
                    steps{sh 'sleep 10'}

                }
                stage('parallel 2'){
                    steps{sh 'sleep 10'}
                } 
            }
        }

    }
}