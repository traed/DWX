FROM node:alpine
RUN npm install -g sass

CMD if [ $WATCH -eq 1 ]; then sass --watch /sass:/css; else sass --update /sass:/css; fi