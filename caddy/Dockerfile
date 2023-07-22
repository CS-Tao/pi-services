FROM caddy:2.7-builder AS builder

ARG BUILD_VPN_PROXY

ENV https_proxy ${BUILD_VPN_PROXY}
ENV http_proxy ${BUILD_VPN_PROXY}
RUN xcaddy build --with github.com/caddy-dns/alidns

FROM caddy:2.7

COPY --from=builder /usr/bin/caddy /usr/bin/caddy
