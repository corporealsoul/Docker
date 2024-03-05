FROM node

ENV MONGO_DB_USERNAME=admin \
    MONGO_DB_PWD=password

RUN mkdir -p /home/app

COPY ./CLI-Interactive-Nodejs-2024 /home/app

WORKDIR /home/app

EXPOSE 3000

CMD ["node", "/home/app/app.js"]


# PS D:\GITRepos\Docker\YEAR2020\TRAINING2020-Oct22-00> docker build -t node-app .
# PS D:\GITRepos\Docker\YEAR2020\TRAINING2020-Oct22-00> docker run node-app