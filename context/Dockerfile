# phlax/iconic
#
# VERSION       0.0.1


ARG BUILD_FROM=phlax/iconic-base

# Root stage
FROM $BUILD_FROM

RUN cd /app/nvm/versions/node/v12.18.2/lib/ \
	&& sed -i "s/puppeteer.launch();/puppeteer.launch({args: [\"--no-sandbox\"]});/g" node_modules/svgexport/render.js
COPY ./createicon /app/bin/createicon

USER puppeteer
