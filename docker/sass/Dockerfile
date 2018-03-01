FROM ruby:alpine
RUN apk update && apk add build-base
RUN gem install sass

CMD if [ $WATCH -eq 1 ]; then sass --watch /sass:/css; else sass --update /sass:/css; fi