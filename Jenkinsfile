pipeline {
    agent any
    stages{
        stage('Etapa de construccion de aplicacion'){
            agent{
                docker{
                    image 'node:alpine3.20'
                }
            }
            stage('install'){
                steps{
                    sh 'npm install'
                }
            }
        }
    }
}
