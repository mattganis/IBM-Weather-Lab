# IBM-Weather-Lab
Optional Container for IBM JumpStart Node-Red Weather Lab


Prereq's - must have Docker installed on your workstation see: [Docker Install](https://docs.docker.com/get-docker/)

* to Build the container use:

`docker build -t weatherlab .`   -    (don't forget the ending dot)

* To execute the container use:

`docker run -it -v ~/data:/flows -p 1880:1880 weatherlab`
(this will start the containter and automatically run node-red)

* if you want to start node manually (from inside the container), use:

`docker run -it -v ~/data:/flows -p 1880:1880 weatherlab /bin/bash`
