FROM node:8.9.4
MAINTAINER Chris wininger <chris.wininger@gmail.com>

# include our source
ADD ./docker-source/front_end_infinite /front_end_infinite
ADD ./docker-source/resources /resources

# initialize the software
RUN cp /resources/.env /front_end_infinite/
RUN cd /front_end_infinite && npm install
WORKDIR /front_end_infinite
CMD ["npm", "run", "start"]
EXPOSE 3004
