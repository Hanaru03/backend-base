pipeline {
    agent any 
    stages {
        stage('etapa de construccion de aplicacion'){
            agent {
                docker {
                    image 'alpine3.20'
                }
            }
            steps{
                echo 'Hola Mundo desde consola de jenkins'
                sh 'echo "Hola Mundo desde el terminal"'
                sh 'npm install'
            }
        }
    }
}
