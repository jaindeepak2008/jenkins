pipeline {
    agent any

    environment {                           // Declaring at Pipeline will allow all the stages to access this variable
        ENV_URL = "pipeline.global.com"
    }

    stages {
        stage('One'){
            steps {
                echo "I am stage One"
                echo "Env URL is ${ENV_URL}"
            }
        }

        stage('Two'){
            steps {
                echo "I am stage Two"
            }
        }

        stage('Three'){
            steps {
                    sh '''
                        echo hello World
                        echo Hai World
                        echo I am using Pipeline Syntax Generator
                    '''
                }
        }

    }
}