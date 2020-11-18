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
        stage('Deploy') {
                steps{
                    //nexusPublisher nexusInstanceId: 'nexus-server', nexusRepositoryId: 'maven-snapshots', packages: [[$class: 'MavenPackage', mavenAssetList: [], mavenCoordinate: [artifactId: 'big-data-deploy-example', groupId: 'org.example', packaging: 'tar.gz', version: '1.0-SNAPSHOT']]]
                }
        }
    }
}