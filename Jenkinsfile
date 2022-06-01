pipeline{
    agent any
    stages{
        stage('stage1'){
            steps{
                CatchError(buildResult: 'UNSTABLE',message:'ERROR',stageResult:'FAILURE'){
                    sh 'exit0'
                }
            }
        }
        stage('stage2'){
            steps{
                echo 'Running stage2'
            }
        }
        
    }
}