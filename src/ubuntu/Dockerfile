FROM ubuntu

COPY README.md /
COPY script.sh /

RUN apt-get update \
  && apt-get install --yes --no-install-recommends \
  iputils-ping \
  && mkdir /var/log/ping-log

CMD ["/script.sh"]  