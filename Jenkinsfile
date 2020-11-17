pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
               echo 'this is deploy'
               sh 'mvn clean deploy -Dmaven.test.skip=true'

            }
        }
    }
}