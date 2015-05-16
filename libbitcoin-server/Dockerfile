FROM       teneighty/libbitcoin-base
MAINTAINER Tim Horton <tmhorton@gmail.com>

RUN wget https://raw.githubusercontent.com/libbitcoin/libbitcoin-server/version2/install.sh
RUN chmod +x install.sh
RUN ./install.sh

# The query service endpoint, defaults to 'tcp://*:9091'.
EXPOSE 9091
# The heartbeat endpoint, defaults to 'tcp://*:9092'.
EXPOSE 9092
# The block publishing service endpoint, defaults to 'tcp://*:9093'.
EXPOSE 9093
# The transaction publishing service endpoint, defaults to 'tcp://*:9094'.
EXPOSE 9094

# Init & run libbitcoin-server
# VOLUME /data
# RUN cd /data && bs -i
# CMD ["bs"]
