pipeline {
    agent any
    environment {
       NEXUS_CREDENCIAL_ID = "nexus-credentials"
       VERSION = readMavenPom().getVersion()

    }
    stages {
        stage('publish') {
            steps {
               echo 'this is deploy'
               sh '/opt/maven/bin/mvn -B -DskipTests clean deploy'
            }
        }
        stage('deploy'){

            steps {
                withCredentials([usernamePassword(credentialsId: 'nexus-cred', passwordVariable: 'pass', usernameVariable: 'user')]) {
                        sh '/var/lib/jenkins/deploy.sh'
                }
            }
        }

    }



}