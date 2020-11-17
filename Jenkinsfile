pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
               echo 'this is deploy'
               //sh 'mvn -B -DskipTests clean package'
               withMaven(maven : 'apache-maven-3.6.3') {
                     sh 'mvn -version'
               }
            }
        }
    }
}