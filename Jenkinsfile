pipeline{
    agent any

    stages{
        stage('Trigger'){
            steps{
                withCredentials([usernamePassword(credentialsId: 'trigger-credentials', passwordVariable: 'PASSWORD_VAR', usernameVariable: 'USERNAME_VAR')]){
                       sh 'curl -k -X POST http://34.219.158.3:8080/job/free-style/build --user  ${USERNAME_VAR}:${PASSWORD_VAR}'
                }
            }
        }
    }
}