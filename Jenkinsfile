pipeline {
    agent any

    stages {
        stage('cd master branch') {
            steps {
              git 'https://github.com/efsavage/hello-world-war.git'
            }
        }
         stage('cb') {
            steps {
               sh 'mvn install'
            }
        }
         stage('cdp') {
             steps
             {
        sh 'cp target/hello-world-war-1.0.0.war /opt/apache-tomcat-9.0.56/webapps'
            }
        }
    }
 }

