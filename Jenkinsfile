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

                    // this is for stage environment
                    if (params.env == 'stage'){
                        echo 'This is my'+ ${params.env}+ 'Environmet'
                        echo 'I am running in'+ ${params.env} + 'Evnironment'

                    }

                    // this is for prod environment
                    if (params.env == 'prod'){
                        echo  " this is my ${params.env} Environment"
                        echo  "I am running in ${params.env} Evnironment"

                    }
                }
            }
        }
        stage ('Trigger other Job') {
            steps {
                build job: "my-first-job"

            }
        }
    }
}
