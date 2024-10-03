pipeline {
    agent any 
    stages {
        stage('etapa de construccion de aplicacion'){
            agent {
                docker {
                    image 'alpine3.20'
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
