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
sudo ls
su -
apt-get update
apt-get install sudo
sudo ls
sudo apt update
sudo apt install python3-pip python3-dev
it will asks do you want to continue [y/n] we should give y to install
sudo -H pip3 install --upgrade pip
sudo -H pip3 install virtualenv
mkdir ~/myproject_dir
cd ~/myproject_dir
virtualenv myproject_env
source myproject_env/bin/activate
pip install jupyter
jupyter notebook --allow-root

```

Refrences:
Docker: 

  installation-> https://docs.docker.com/docker-for-windows/install/
  
  errors-> https://www.bing.com/videos/search?view=detail&mid=C12FF81E191DA0CA296AC12FF81E191DA0CA296A&q=docker
  
  ubuntu -> http://www.servermom.org/pull-docker-images-run-docker-containers/3225/#:~:text=To%20pull%20an%20image%2C%20use%20%E2%80%9C%20docker%20pull,your%20server%2C%20use%20%E2%80%9C%20docker%20images%20%E2%80%9D%20command
  
  python -> https://www.datasciencelearner.com/install-and-run-python-in-docker-container/
  In another cmd:
docker run -p 8888:8888 jupyter/minimal-notebook

**Error:**
```
1.jupyter notebook,--allow-root,jupyter notebook --no-browser --port=8888,local:8888****

2.jupyter notebook --allow-root then we got - we cannot connect to localhost

3.docker run -p 8888:8888 jupyter (opens latest, but not available)
```
