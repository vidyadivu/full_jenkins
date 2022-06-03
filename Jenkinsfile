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
                        echo 'this is dev env'
                    }
                    if (params.env== 'prod'){
                        echo 'this is prod env'
                    }
                    if (params.env== 'stage'){
                        echo 'this is stage env'
                    }
                }
            }
        }
    }
}
