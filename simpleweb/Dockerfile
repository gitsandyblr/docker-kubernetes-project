# use base images
FROM node:alpine

#putting files in user folder in box so to avoid overriding of existing folders
WORKDIR /usr/app

COPY ./package.json ./

# install dependencis
RUN npm install

# ./ ./ => copy everything from current working dir to working dir of docker
COPY ./ ./

#tell image what to do when started
CMD ["npm", "start"]