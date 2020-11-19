pipeline {
    agent any
    environment {
       NEXUS_CREDENCIAL_ID = "nexus-credentials"
    }
    stages {
        stage('Build') {
            steps {
               echo 'this is deploy'
                withMaven(maven: 'M3', mavenSettingsConfig: 'maven-setting') {
                       sh '/opt/maven/bin/mvn -B -DskipTests clean deploy'
                   }

            }
        }

    }
}