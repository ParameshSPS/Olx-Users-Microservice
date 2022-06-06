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
         stage('test report using jacoco') {
            steps {
                echo 'jacoco'
            }
        }
        stage('building docker image') {
            steps {
                echo 'building docker image'
            }
        }
    }
}
