pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    try {
                        sh '''
                        ./mvnw clean package -DskipTests
                        '''
                    } catch (exec) {
                        throw exec
                    } finally {
                    }
                }

            }
        }
    }
}