pipeline{
    agent any
    parameters {
        choice choices: ["dev","stage","prod"], description: 'My env', name: 'env'
    }
    stages {

        stage ('Running with environments'){
            steps {
                script {
                    if (params.env== 'dev'){
                        echo "${params.env} environment"
                    }
                    if (params.env== 'prod'){
                        echo "${params.env} env"
                    }
                    if (params.env== 'stage'){
                        echo 'this is stage env'
                    }
                }
            }
        }
        post {
            success {
                script {
                    echo "${params.env} environment is success"
                }
            }
        }
    }
}
