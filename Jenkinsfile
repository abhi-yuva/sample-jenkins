pipeline {
    agent { label 'agent1' }
    
    parameters {
        choice choices: ['dev','stage','prod'], description: 'My Environments', name: 'Environment'
    }

    stages {
        stage('First Stage') {
            steps {
                echo "this is my frist stage"
            }
        }

        stage('2nd stage') {
            steps {
                echo "this is my Second stage"
            }
        }
        stage('3rd stage') {
            steps {
                echo "this is my Second stage"
            }
        }
        stage('4th stage') {
            steps {
                echo "this is my Second stage"
            }
        }
    }
}
