pipeline {
     agent any 
       stages {
          stage (checkout) {
              step {
                  git 'https://github.com/shubhmatre/Jenks1.git'
                    }
                 }
          stage (compile) {
               step {
                  sh 'mvn install'
                    }
                      }
           stage (deployment) {
                step {
                 sh 'cp target/Jenks1 /home/shubham/Documents/devops/apache-tomcat-9.0.93/webapps'
}
}
}
}
