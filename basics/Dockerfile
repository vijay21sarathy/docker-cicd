FROM node:4.6 as unittest
RUN sleep 5
RUN echo " Unit Test"

FROM node:4.6 as code coverage
RUN sleep 5
RUN echo " code covergae"

FROM node:4.6 as final
WORKDIR /app
ADD . /app

RUN echo " final artifact"
RUN npm install
EXPOSE 3000
CMD npm start
