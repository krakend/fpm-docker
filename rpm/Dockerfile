FROM centos:7
maintainer dortiz@devops.faith

RUN yum install -y \
	ruby-devel \
	gcc \
	make \
	ruby \
	rpm-build \
	rpm-sign && yum clean all

RUN gem install fpm -v 1.9.3 --no-ri --no-rdoc

VOLUME [ "/tmp/fpm" ]
WORKDIR /tmp/fpm

ENTRYPOINT [ "/usr/local/bin/fpm" ]
CMD [ "--help" ]
