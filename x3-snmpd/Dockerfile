FROM alpine

RUN apk update && apk add -u bash && apk add -u net-snmp

ADD snmpd.conf /etc/snmp/snmpd.conf
ADD run.sh /run.sh

EXPOSE 161/udp
ENTRYPOINT ["/bin/bash", "/run.sh"]
