pipeline {
    agent any

    stages {
        stage('check out') {
            steps {
               git 'https://github.com/ParameshSPS/Olx-Users-Microservice.git' 
            }
        }
        stage('compile') {
            steps {
                echo 'compiling'
            }
        }
        stage('running') {
            steps {
                echo 'running'
            }
        }
    }
}
