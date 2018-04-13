# jenkinsfile
# This is NodeJS Code used for testing Jenkins
Jenkinsfile (Declarative Pipeline)
pipeline {
    agent { docker { image 'node:6.3' } }
    stages {
        stage('build') {
            steps {
                sh 'npm --version'
            }
        }
    }
}
