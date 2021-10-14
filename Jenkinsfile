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
        stage('Validar Kiuwan'){
            steps{
                sh 'echo "validar kiuwan (en construcción)"'
            }
        }
        stage('Pruebas unitarias'){
            steps{
                sh 'echo "Pruebas unitarias (en construcción)"'
            }
        }
        stage('Generación APK'){
            steps{
                sh 'ng build'
            }
        }
        stage('Pruebas funcionales'){
            steps{
                sh 'echo "Pruebas funcionales (en construcción)"'
            }
        }
        stage('Pruebas de carga'){
            steps{
                sh 'echo "Pruebas de carga (en construcción)"'
            }
        }
        stage('SauceLab'){
            steps{
                sh 'echo "SauceLab (en construcción)"'
            }
        }
        stage('Despliegue en Google Play'){
            steps{
                sh 'echo "Despliegue en Google Play (en construcción)"'
            }
        }
    }
}