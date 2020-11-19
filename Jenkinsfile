pipeline {
    agent any
    environment {
       NEXUS_CREDENCIAL_ID = "nexus-credentials"
    }
    stages {
        stage('publish') {
            steps {
               echo 'this is deploy'
               sh '/opt/maven/bin/mvn -B -DskipTests clean deploy'
            }
        }

    }
}