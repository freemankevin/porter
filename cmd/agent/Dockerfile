FROM alpine
WORKDIR /
RUN apk update && apk add iptables
ARG TARGETOS
ARG TARGETARCH
COPY bin/agent-${TARGETOS}-${TARGETARCH} agent
ENTRYPOINT ["/agent"]