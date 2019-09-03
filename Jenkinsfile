pipeline {
    agent any

    stages {
        stage('clone') {
            steps {
                git url : 'https://github.com/Diovane1103/TemaFinal1.git'
            }
        }
        stage('build') {
            steps {
                sh 'gradle clean build'
            }
        }
    }
}
