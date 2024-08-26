FROM wangdongbing/alpine:3.20.2

LABEL maintainer="wangdongbing <2987794446@qq.com>"

RUN apk add --no-cache frp@community=0.60.0-r0\
    && rm -rfv /usr/bin/frps /etc/frp/frps.toml

ENTRYPOINT ["/usr/bin/frpc"]

CMD ["-c", "/etc/frp/frpc.toml"]