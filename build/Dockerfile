FROM quay.io/operator-framework/helm-operator:latest
LABEL name="Cockroach DB Operator"
LABEL vendor="Cockroach Labs"
LABEL version="19.2.2"
LABEL release="1"
LABEL summary="CockroachDB is a Distributed SQL database."
LABEL description="CockroachDB is a PostgreSQL wire-compatable Distributed SQL database."
COPY watches.yaml ${HOME}/watches.yaml
COPY helm-charts/ ${HOME}/helm-charts/
USER root
RUN mkdir -p /licenses
COPY LICENSE /licenses/
USER 1000
