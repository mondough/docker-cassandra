# Spotify Cassandra 2.1.8 Single Node Image
#
# VERSION               0.1
#
# Starts a Cassandra instance constituting a one node cluster.

FROM mondough/docker-cassandra:base

USER root

# Place single-node startup-config script
ADD scripts/cassandra-singlenode.sh /usr/local/bin/cassandra-singlenode

# Start Cassandra
ENTRYPOINT ["cassandra-singlenode"]
