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
                        echo 'This is my'+ ${params.env}+ 'Environmet'
                        echo 'I am running in'+ ${params.env} + 'Evnironment'

                    }

                    if (params.env == 'stage'){
                        echo 'This is my'+ ${params.env}+ 'Environmet'
                        echo 'I am running in'+ ${params.env} + 'Evnironment'

                    }

                    if (params.env == 'prod'){
                        echo 'This is my'+ ${params.env}+ 'Environmet'
                        echo 'I am running in'+ ${params.env} + 'Evnironment'

                    }
                }
            }
        }
    }
}
