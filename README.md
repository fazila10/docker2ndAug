# docker2ndAug

**1)Docker installation.**
   
   a)From docks.docker.com we have downloaded docker.
   
   b)After downloaded we got error while installing (Docker desktop requires server services to be enabled)
   
              steps for error rectification
                    1)control panel->programs and features->Turn Windows features on or off-> enable  Hyper-V
                    2)in search type services.msc -> server -> automatic/Manual
                    
**2)Creating ubuntu image**
open cmd prompt
```
               docker pull ubuntu                   #pulls the image
               docker ps -l                          #list all images
               docker run -i -t ubuntu /bin/bash      #runs the ubuntu image
```
**3)setup python notebook**
a)Installing python
```
docker run -ti -d ubuntu: latest            #running ubuntu
docker ps                                   #To get images
apt-get update                              #Updating ubuntu to latest version 
apt-get install python3                     #Install python 
```

Refrences:
Docker: 

  installation-> https://docs.docker.com/docker-for-windows/install/
  
  errors-> https://www.bing.com/videos/search?view=detail&mid=C12FF81E191DA0CA296AC12FF81E191DA0CA296A&q=docker
  
  ubuntu -> http://www.servermom.org/pull-docker-images-run-docker-containers/3225/#:~:text=To%20pull%20an%20image%2C%20use%20%E2%80%9C%20docker%20pull,your%20server%2C%20use%20%E2%80%9C%20docker%20images%20%E2%80%9D%20command
  
  python -> https://www.datasciencelearner.com/install-and-run-python-in-docker-container/
