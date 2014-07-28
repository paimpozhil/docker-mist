docker-mist
===========

### Easy way to test drive Mist.io's public opensource code or to start a dev environment based on this

```
git clone https://github.com/paimpozhil/docker-mist.git 
cd docker-mist
docker build -t mistio .
docker run -td -p 8000:8000 mistio 
```


Now you can easily see the Mist running in your interface

#### http://[server/host ip]:8000 

Please note this has no login/authentication whatever for now. Please use it only on internal network 

Or use an Nginx proxy or some other auth mechanism if you prefer to use it in production which may not be advised at the moment.

This code ONLY allows me to manage inventory but not to use shell or monitoring features and require login to http://mist.io for some reason.


Hope this helped you to have a look the Mist.io closely.



### if youd like develop/contribute you may need a shell please use the following command and cd /home/mist 
```
docker run -ti -p 8000:8000 mistio /bin/bash
```


