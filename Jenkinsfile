pipeline {
    agent any
    stages{
        stage('port 8080 testing'){
            steps{
                script{
                    if(env.HUDSON_URL.contains('8080')){
                        echo 'Jenkins is running on 8080'
                    }
                    else{
                        echo 'Jenkins is not running on 8080'
                    }
                }
            }
        }
    }
}
                 
        
                
            