Tasks To Be Performed:
1. Pull Ubuntu container   
2. Run this container and map port 80 on the local
3. Install Apache2 on this container
4. Check if you are able to access the Apache page on your browser


Step 1:
execute this command it will pull latest ubuntu container in docker
 "docker pull ubuntu:latest"



Step 2:
* Starts the container in interactive mode (-it)
* Maps port 80 of your local machine to port 80 inside the container
* Names the container ubuntu-apache
"docker run -it -p 80:80 --name ubuntu-apache ubuntu:latest"
* And this command will navigate the inside the docker container


 Step 3:
* Now Update the container and install the apache2 with this command 
 "apt update"
 "apt install apache2 -y"

Step 4:
* Now start and check status of the apache2 service with this command
  "service apache2 start"
  "service apache2 status"
(Press q to quit the status view) 

Step 5:
* Access the Apache page on your browser with your Ip or localhost

