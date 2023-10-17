from node:20-alpine

RUN apk add --no-cache curl bash nodejs


RUN npm install -g --unsafe-perm node-red

WORKDIR /root/.node-red

RUN npm install node-red-dashboard
RUN npm install node-red-contrib-ui-media
RUN npm install node-red-contrib-web-worldmap

CMD ["node-red","-D","flowFile=/flows/weatherlab.flows"]

