FROM node:8.9.4
MAINTAINER Chris wininger <chris.wininger@gmail.com>

# include our source
ADD ./docker-source/infinite /infinite
ADD ./docker-source/resources /resources

# initialize the software
RUN cp /resources/.env /infinite/
RUN cd /infinite && npm install
WORKDIR /infinite
CMD ["npm", "run", "start-docker"]
EXPOSE 3003
