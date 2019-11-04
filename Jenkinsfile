pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    try {
                        sh '''
                        ./mvnw clean package --stacktrace
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