pipeline {
    agent any
    //environment {
    //    NEXUS_CREDENCIAL_ID = "nexus-credentials"
   // }
    stages {
        stage('Build') {
            steps {
               echo 'this is deploy'
               sh '/opt/maven/bin/mvn -B -DskipTests clean deploy'


            }
        }

    }
}