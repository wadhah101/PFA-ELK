FROM thehiveproject/cortex:3.1.4-1

COPY ./application.conf /etc/cortex/application.conf

USER root
RUN apt update && apt install -y python3-pip && rm -rf /var/lib/apt/lists/*
RUN pip3 install ldap3 requests
RUN pip3 install cortexutils
