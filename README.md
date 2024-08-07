# gitea with docker-compose
[![Build Status](https://raw.githubusercontent.com/ariadata/ariadata-files/main/public-assets/images/ariadata_logo.png)](https://ariadata.co)

![](https://img.shields.io/github/stars/ariadata/dc-gitea.svg)
![](https://img.shields.io/github/watchers/ariadata/dc-gitea.svg)
![](https://img.shields.io/github/forks/ariadata/dc-gitea.svg)

### This needs : [dockerhost](https://github.com/ariadata/dockerhost-sh) + [nginx-proxy-manager](https://github.com/ariadata/dc-nginxproxymanager)

---
#### 1- Clone these repository to your system :
```sh
git clone https://github.com/ariadata/dc-gitea.git
```
#### 2- cd into created folder :
```sh
cd dc-gitea
```
#### 3- edit `docker-compose.yml` ( lines : 20,38,40 ):
#### 4- Run docker-compose file by using :
```sh
docker-compose up -d
```
#### 5- Goto Nginx-Proxy-Manager admin panel and add this stack as proxy-host :
> Domain : `Your-FQDN`
> 
> Schema : `http`
> 
> Name or IP : `gitea`
> 
> Port : `3000`
>
> SSL is Recommended!

#### 6- Goto gitea setup page : 
>  `http://Your-FQDN/`
>  
>  or 
>  
>  `http://Your-IP:3000`

#### 7- Important Parts in Setup :
> Gitea HTTP Listen Port : `3000`
>
> Gitea Base URL : `https://Your-FQDN/` or with `http` if not configured
> 
> Fill Administrator part at the end of setup page!

Done!


