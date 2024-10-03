pipeline {
    agent any 
    environment{
        NPM_CONFIG_CAFHE = "${WORKSPACE}/.npm"
    }
    
    stages {
        stage('etapa de construccion de aplicacion'){
            agent {
                docker {
                    image 'node:alpine3.20'
                }
            } stages{
                stage('install'){
                    steps{
                         sh 'npm install'
                    }                    
                }
            }
        }
    }
}
