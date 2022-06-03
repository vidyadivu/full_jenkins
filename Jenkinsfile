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
                        echo 'if it is true.print dev environment'
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
                echo "${params.env} is success"
            }
        }
    }
}
