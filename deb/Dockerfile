FROM ubuntu:16.04
LABEL maintainer="dortiz@devops.faith"

RUN apt-get update && apt-get install -y \
	ruby-dev \
	gcc \
	make \
	ruby \
	&& rm -rf /var/lib/apt/lists/*

RUN gem install fpm -v 1.9.3 --no-ri --no-rdoc

VOLUME [ "/tmp/fpm" ]
WORKDIR /tmp/fpm

ENTRYPOINT [ "/usr/local/bin/fpm" ]
CMD [ "--help" ]
