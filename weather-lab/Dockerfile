from node:12-alpine

RUN apk add --no-cache curl bash nodejs

RUN mkdir -p /root/.node-red
RUN mkdir -p /root/red
VOLUME /root/.node-red

RUN npm install -g --unsafe-perm node-red

WORKDIR /root/.node-red

# CMD ["npm","i","--g --unsafe-perm node-red"]

RUN npm install node-red-dashboard
RUN npm install node-red-contrib-ui-media
RUN npm install node-red-contrib-web-worldmap

