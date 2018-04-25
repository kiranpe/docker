pipeline {
      agent any 
      
      stages {
         stage ('Test') {
               steps {
                  sh "sudo docker pull nginx:latest"
                  sh "sudo docker run --name nginx -p 8090:80 -d -it nginx"
               }
         }
      }
} 
    
