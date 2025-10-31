pipeline {
    agent any

    stages {
        stage('Build') {
            agent {
                docker {
                    image 'node:24.11.0-alpine3.22'
                    reuseNode true
                }
            }
            steps {
                sh '''
                    ls -la
                    mvn -v
                '''
            }
        }
    }
}
