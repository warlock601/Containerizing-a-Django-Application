## Containerizing-a-Django-Web-Application
We'll containarize a web-app using Docker. <br />
We'll use an Ubuntu image on an EC2 instance, SSH into it and then install and configure Docker on it s follows: <br />
 ```bash
  sudo apt-get update 
  sudo apt-get install docker
  sudo systemctl start docker
  sudo usermod -aG docker ubuntu      # this command will do user modification as it will add user "ubuntu" in "docker" users group
  docker run hello-wrold              # this will fist download a default image and then display Hello-Docker 
```
Note: If we don't use "sudo usermod -aG docker ubuntu" command, then we will need to execute docker commands using sudo. <br />
Then build a [Docker file]() to pull the ubuntu base-image and then install python dependencies so that we can run our web-app. 
