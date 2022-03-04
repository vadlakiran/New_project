FROM node:9.6.1

ENV PATH /usr/src/app/.bin:$PATH
RUN mkdir -p /usr/src/app
WORKDIR c
COPY . /usr/src/app

RUN rm -rf node_modules/*
RUN chown -R /usr/src/app/package.json
RUN chown -R /usr/src/app/yarn.lock.json
RUN chmod 777 /usr/src/app/package.json
RUN chmod 777 /usr/src/app/yarn.lock.json
RUN npm install

EXPOSE 3000 

# START app
#CMD ["/usr/local/bin/node", "/usr/src/app/src/App.js"]
ENTRYPOINT npm start
