pipeline {
    agent { docker { image 'gradle:4.4.1' } }
    stages {
        stage('build') {
            steps {
                sh 'gradle --version'
            }
        }
    }
}