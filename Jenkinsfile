pipeline {
    agent any
    
    parameters {
        choice choices: ['dev','stage','prod'], description: 'My Environments', name: 'env'
    }
    stages{
        stage ('Running with Environments') {
            steps{
                script{
                    // this is for dev environment
                    if (params.env == 'dev'){
                        echo 'This is my Dev Environmet'
                        echo 'I am running in Dev Evnironment'

                    }

                    if (params.env == 'stage'){
                        echo 'This is my stage Environmet'
                        echo 'I am running in stage Evnironment'

                    }

                    if (params.env == 'prod'){
                        echo 'This is my Prod Environmet'
                        echo 'I am running in Prod Evnironment'

                    }
                }
            }
        }
    }
}
