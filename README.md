# docker-armhf-deluge
Deluge is a torrent client. One of the best things about it is its highly client-server oriented, allowing you to remote control a deluge server from your desktop deluge app or using the web interface (deluge-web). 

# how to build
docker build -t vl0ms/armhf-deluge .

# how to pull
docker pull vl0ms/armhf-deluge

# how to start
docker run -d --restart=always -v /your/config/folder:/config -v /your/data/folder:/data -p 58846:58846 -p 8112:8112 --name=deluge vl0ms/armhf-deluge
