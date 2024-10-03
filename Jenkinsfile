pipeline {
    agent any
    environment{
        NPM_CONFIG_CACHE = "${WORKSPACE}/.npm"
    }
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
