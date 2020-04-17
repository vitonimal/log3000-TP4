FROM node:latest

RUN apt-get update -qq && apt-get install -qy \ 
    ca-certificates \
    bzip2 \
    curl \
    libfontconfig \
    --no-install-recommends

ENV PUPPETEER_SKIP_DOWNLOAD=false
RUN npm i -g puppeteer
ADD . /app
WORKDIR /app
CMD ["/app/tests.sh"]
