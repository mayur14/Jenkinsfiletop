pipeline {
    agent any
    environment {
        name = 'mayur'
    }
    parameters {
        string(name: 'person', defaultValue: 'mayur', description: 'what todu fodu you wanna do today')
        booleanParam(name: 'isDev', defaultValue: 'true', description: '')
        choice(name: 'title',  choices: ['Dev', 'Tester', 'DevOps', 'Admin'], description: 'what todu fodu you wanna do today')
    } 


    stages {
        stage('Build') {
            steps {
                bat 'echo "%BUILD_ID%"'
                bat 'echo "%name%"'
                bat 'dir'
            }
        }    

        stage('Test') {
        environment {
            name = 'tote'
        }
            steps {
                echo 'Hello World'
                bat 'echo "%name%"'
            }
        }    
        stage('Deploy') {
            steps {
                echo 'Hello World'
                bat 'echo "%person%"'
            }
        }    
    }
        post{
            always {
                echo 'apun toh badshah hai har bar chalega'
            }
            success {
                echo 'success is the only option failure not'
            }
        }
}
