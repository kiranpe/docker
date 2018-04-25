pipeline {
      agent any 
      
      stages {
         stage ('Test') {
               steps {
                  sh "sudo docker pull nginx:latest"
                  sh "sudo docker stop nginx"
                  sh "sudo docker rm nginx"
                  sh "sudo docker run --name nginx -p 8090:80 -d -it nginx"
                  sh "sudo docker cp index.html nginx:/usr/share/nginx/html"
               }
         }
      }
} 
    
