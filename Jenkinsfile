pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
               echo 'this is deploy'
               //sh 'mvn -B -DskipTests clean package'
               sh 'export MAVEN_HOME=/opt/maven'
               sh 'export PATH=$PATH:$MAVEN_HOME/bin'
               sh 'mvn -version'

            }
        }
    }
}