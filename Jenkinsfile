pipeline {
    agent {  docker { image 'bitnami/laravel'}
                } 
    
    environment {
        APP_VERSION = '1'
    }
    stages {
        stage('Build') {
            steps {
                   sh 'php --version'
                   sh 'composer install'
            }
        }
        stage('Test') {
            steps {
                echo 'test Done...2.'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
        post {
                success {
                     echo 'success2'
                }

                failure {
                    echo 'failded11'
                }
            }
        }
    }
}