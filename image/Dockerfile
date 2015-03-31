FROM ubuntu:14.04
MAINTAINER Phusion <info@phusion.nl>

ENV HOME /root
ADD . /build

RUN 1=1 && /build/prepare.sh && \
	/build/system_services.sh && \
	/build/utilities.sh && \
	/build/cleanup.sh

CMD ["/sbin/my_init"]
