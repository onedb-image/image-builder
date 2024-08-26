FROM wangdongbing/alpine:3.20.2

LABEL maintainer="wangdongbing <2987794446@qq.com>"

RUN apk add --no-cache frp@community=0.60.0-r0\
    && rm -rfv /usr/bin/frpc /etc/frp/frpc.toml

ENTRYPOINT ["/usr/bin/frps"]

CMD ["-c", "/etc/frp/frps.toml"]