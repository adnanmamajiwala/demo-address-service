pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    try {
                        sh '''
                        ./mvnw clean package
                        '''
                    } catch (exc) {
                        throw exec
                    } finally {
                    }
                }

            }
        }
    }
}