## 🎨 Ghostty 配置
**位置**：nano ~/.bashrc

```conf
# Clash proxy config
PROXY_HTTP="http://127.0.0.1:7897"
PROXY_SOCKS="socks5://127.0.0.1:7897"

proxy_on() {
    export http_proxy="$PROXY_HTTP"
    export https_proxy="$PROXY_HTTP"
    export HTTP_PROXY="$PROXY_HTTP"
    export HTTPS_PROXY="$PROXY_HTTP"

    export all_proxy="$PROXY_SOCKS"
    export ALL_PROXY="$PROXY_SOCKS"

    echo "终端代理已开启。"
}

proxy_off() {
    unset http_proxy https_proxy all_proxy
    unset HTTP_PROXY HTTPS_PROXY ALL_PROXY
    echo "终端代理已关闭。"
}

proxy_status() {
    echo "http_proxy=$http_proxy"
    echo "https_proxy=$https_proxy"
    echo "all_proxy=$all_proxy"
    echo "HTTP_PROXY=$HTTP_PROXY"
    echo "HTTPS_PROXY=$HTTPS_PROXY"
    echo "ALL_PROXY=$ALL_PROXY"
}

codex_proxy() {
    env \
      ALL_PROXY="$PROXY_SOCKS" \
      all_proxy="$PROXY_SOCKS" \
      HTTPS_PROXY="$PROXY_HTTP" \
      https_proxy="$PROXY_HTTP" \
      HTTP_PROXY="$PROXY_HTTP" \
      http_proxy="$PROXY_HTTP" \
      codex "$@"
}

# 新终端默认关闭代理
unset http_proxy https_proxy all_proxy
unset HTTP_PROXY HTTPS_PROXY ALL_PROXY
```
