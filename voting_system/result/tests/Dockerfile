FROM node:latest

ENV PUPPETEER_SKIP_CHROMIUM_DOWNLOAD=true

RUN apt-get update -qq && apt-get install -qy \ 
    ca-certificates \
    bzip2 \
    curl \
    libfontconfig \
    --no-install-recommends
 # RUN yarn global add phantomjs-prebuilt
RUN npm r -g phantomjs-prebuilt karma-phantomjs-launcher
RUN npm i -g karma-chrome-launcher puppeteer
# RUN npm i -g mkdirp
ADD . /app
WORKDIR /app
CMD ["/app/tests.sh"]
