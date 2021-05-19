FROM ubuntu

RUN apt-get update \
  && apt-get install --yes --no-install-recommends \
  iputils-ping

COPY README.md /

CMD ["ping", "www.google.com"]  