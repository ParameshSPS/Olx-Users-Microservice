pipeline {
    agent any

    stages {
        stage('check out') {
            steps {
               git 'https://github.com/ParameshSPS/Olx-Users-Microservice.git' 
            }
        }
//         stage('compile') {
//             steps {
//                 echo 'compiling'
//             }
//         }
         stage('compile') {
            steps {
                bat 'mvn clean compile'
            }
        }
//         stage('running') {
//             steps {
//                 echo 'running'
//             }
//         }
        stage('running') {
            steps {
                bat 'mvn package'
            }
        }
//          stage('test report using jacoco') {
//             steps {
//                 echo 'jacoco'
//             }
//         }
        stage('test report using jacoco') {
            steps {
                jacoco()
            }
        }
        stage('building docker image') {
            steps {
                echo 'building docker image'
            }
        }
    }
}
