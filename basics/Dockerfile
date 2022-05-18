FROM node:4.6 as unittest
RUN sleep 5
RUN echo " Unit Test"

FROM unitest as codecoverage
RUN sleep 5
RUN echo " code covergae"

FROM codecoverage as final
WORKDIR /app
ADD . /app

RUN echo " final artifact"
RUN npm install
EXPOSE 3000
CMD npm start
