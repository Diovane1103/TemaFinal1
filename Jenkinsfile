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
        stage('JFrog') {
            steps {
                sh 'curl -uadmin:AP5MhsmLzDkCkV4mrwzXgzLpgGz -T .build/libs/desafioFinal-0.0.1-SNAPSHOT.war "http://localhost:8081/artifactory/repo/hello.war"'
            }
        }
    }
}
