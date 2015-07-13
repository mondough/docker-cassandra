# Spotify Cassandra 2.1.8 Cluster Node Image
#
# VERSION               0.1
#
# Expects CASSANDRA_SEEDS and CASSANDRA_TOKEN env variables to be set.
# If CASSANDRA_SEEDS is not set, node acts as its own seed
# If CASSANDRA_TOKEN is not set, startup process is aborted

FROM mondough/docker-cassandra:base

USER root

# Place cluster-node startup-config script
ADD scripts/cassandra-clusternode.sh /usr/local/bin/cassandra-clusternode

# Start Cassandra
ENTRYPOINT ["cassandra-clusternode"]
