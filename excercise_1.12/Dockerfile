FROM node:16

COPY ./material-applications/example-frontend .

RUN node -v && npm -v
RUN npm install
RUN npm run build
RUN npm install -g serve
CMD serve -s -l 5000 build

EXPOSE 5000