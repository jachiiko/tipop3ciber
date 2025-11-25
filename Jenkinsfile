pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Construyendo el proyecto...'
            }
        }

        stage('Test') {
            steps {
                echo 'Ejecutando pruebas...'
            }
        }

        stage('Generate Documentation') {
            steps {
                echo 'Generando documentación con Doxygen...'
                sh 'doxygen Doxyfile'
            }
        }

        stage('Ejecutar script Python') {
            steps {
                echo 'Ejecutando script Python...'
                sh 'python3 app.py'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Desplegando aplicación...'
            }
        }
    }
}
