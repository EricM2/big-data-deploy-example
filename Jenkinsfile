pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
               echo 'this is deploy'
               sh '/opt/maven/bin/mvn -B -DskipTests clean deploy'
               //sh 'mvn '

            }
        }
    }
}