pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
               echo 'this is deploy'
               sh '/opt/maven/bin/mvn -version'
               //sh 'mvn -B -DskipTests clean package'

            }
        }
    }
}