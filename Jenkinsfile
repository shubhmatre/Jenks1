pipeline {
     agent any 
       stages {
          stage (checkout) {
              steps {
                  git 'https://github.com/shubhmatre/Jenks1.git'
                    }
                 }
          stage (compile) {
               steps {
                  sh 'mvn install'
                    }
                      }
           stage (deployment) {
                steps {
                 sh 'cp target/Jenks1 /home/shubham/Documents/devops/apache-tomcat-9.0.93/webapps'
}
}
}
}
