pipeline {
    agent any

    stages {

        stage('Clonar repositorio') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/jachiiko/tipop3ciber.git'
            }
        }

        stage('Generar documentación con Doxygen') {
            steps {
                sh 'doxygen Doxyfile'
            }
        }

        stage('Ejecutar script Python') {
            steps {
                sh 'python3 app.py'
            }
        }
    }
}

