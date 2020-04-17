FROM node:latest
<<<<<<< HEAD

ENV PUPPETEER_SKIP_CHROMIUM_DOWNLOAD=true
=======
>>>>>>> 79319a39588f2cbf39ea1ad6c24502419c19a742

RUN apt-get update -qq && apt-get install -qy \ 
    ca-certificates \
    bzip2 \
    curl \
    libfontconfig \
    --no-install-recommends
<<<<<<< HEAD
 # RUN yarn global add phantomjs-prebuilt
RUN npm r -g phantomjs-prebuilt karma-phantomjs-launcher
RUN npm i -g karma-chrome-launcher puppeteer
# RUN npm i -g mkdirp
=======

ENV PUPPETEER_SKIP_DOWNLOAD=false
RUN npm i -g puppeteer
>>>>>>> 79319a39588f2cbf39ea1ad6c24502419c19a742
ADD . /app
WORKDIR /app
CMD ["/app/tests.sh"]
