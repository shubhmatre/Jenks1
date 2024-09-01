pipeline {
        agent{
        label 'slave'
        }
        stages {
            stage('Checkout') {
                steps {
                        checkout scm
                      }}
                stage('Build') {
                   steps {
                          sh 'JAVA_HOME=/home/grras/main/jdk-11.0.20 /home/grras/main/apache-maven-3.9.4/bin/mvn install'
                         }}
                stage('Deployment'){
                    steps {
                        sh 'cp target/Jenks1.war /home/grras/main/apache-tomcat-9.0.79/webapps'
                        }}
}}
~                
