pipeline{
    agent any
    tools {
        nodejs '16.11.0'
    }
    options{
        timeout(time:2, unit:'MINUTES')
    }
    stages{
        stage('Instalación de dependencias'){
            steps{
                sh 'npm install'
            }
        }
        stage('Compilación de la app'){
            steps{
                sh 'npm build'
            }
        }
    }
}