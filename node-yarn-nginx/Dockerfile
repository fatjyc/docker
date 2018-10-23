FROM nginx:alpine


# Avoid ERROR: invoke-rc.d: policy-rc.d denied execution of start.
RUN echo "#!/bin/sh\nexit 0" > /usr/sbin/policy-rc.d

# Install Node.js 8.10.0 LTS and NPM
RUN apk add --update-cache nodejs nodejs-npm --repository http://dl-3.alpinelinux.org/alpine/edge/main/

# Install Yarn Package Manager 1.5.1
RUN apk add --update-cache yarn --repository http://dl-3.alpinelinux.org/alpine/edge/community/

CMD ["node", "--version"]
