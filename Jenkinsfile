pipeline {
    agent any

    stages {
        stage('Bulid') {
            agent{
                docker {
                    image 'node: 18-alpine'
                    reuseNode true

                }                

                }
                

            }
             
            steps {
               sh '''
               ls -la
               node --version
               npm --version
               npm ci
               npm run buid
               ls -la

               '''
            }
        }
    }

