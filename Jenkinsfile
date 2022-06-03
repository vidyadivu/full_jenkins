pipeline{
    agent any
    parameters{
        choice choices: ["dev","stage","prod"], description: "My env", name: "env"
    }
    stages('Running environment variables'){
        stage{
            steps{
                script{
                    if(params.env=='dev'){
                        echo 'this is dev env'
                    }
                    if(params.env=='prod'){
                        echo 'this is prod env'
                    }
                }
            }
        }
    }
}
