pipeline {
    agent any
    parameters {
        choice choices: ["dev","stage","prod"], description: 'My env', name: 'env'
    }
    stages {

        stage ('Running with environments'){
          
            steps {
                script {
                    if (params.env== 'dev'){
                        echo 'if it is true then print dev environment'
                    }
                    else {
                        echo ' print prod env'
                    
                    }
                }
            }
        }
    }
    post {
        success{
            script{
                echo 'dev env is success'
            }
        }
        failure{
            script{
                echo 'prod env is failed'
            }
        }
    }
}
