pipeline {
    agent any

    stages {
        stage('Build') {
            agent {
                docker {
                    image 'maven:3.3-jdk-8'
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
