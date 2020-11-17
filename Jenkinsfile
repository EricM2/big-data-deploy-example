pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
               echo 'this is deploy'
               //sh 'mvn -B -DskipTests clean package'
               sh 'mvn -version'

            }
        }
    }
}