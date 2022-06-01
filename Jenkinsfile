pipeline {
    agent any
    parameters {
        booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')
    }
    stages {
        stage('Stage1') {
            when {
              expression { return params.TOGGLE }
            }
            steps {
                  echo 'Testing'
            }
        }
    }
}