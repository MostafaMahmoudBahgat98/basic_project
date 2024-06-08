pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    docker.build('flask-app')
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    docker.image('flask-app').inside {
                        sh 'python -m unittest discover -s tests'
                    }
                }
            }
        }

        stage('Deploy') {
            steps {
                script {
                    docker.image('flask-app').run('-p 5000:5000')
                }
            }
        }
    }
}

