pipeline {
    agent agents
    stages{
        stage('stage1'){
            steps{echo 'stage1'}
        }
        stage('stage2'){
            steps{echo 'stage2'}
        }
    }
    post{
        always{echo 'post stage'}
    }
}