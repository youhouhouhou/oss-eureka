
FROM ${docker.registry}/java:oracle-8u101-jdk-alpine

VOLUME /tmp
VOLUME ["/root/data"]











ADD entrypoint.sh /root/
RUN chmod 755 /root/*.sh
ADD	*-exec.jar /root/
RUN touch /root/*-exec.jar

EXPOSE 8761
USER root
WORKDIR /root/
ENTRYPOINT ["/root/entrypoint.sh"]
CMD []
