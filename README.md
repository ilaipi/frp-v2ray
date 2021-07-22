# frp-v2ray
use frp to proxy v2ray

## 使用

在项目的Settings - Secrets中设置以下参数：

```
VMESS_PORT   # v2ray 的运行端口

SERVER_ADDR  # frps 服务地址
SERVER_PORT  # frps 服务监听端口
FRP_TOKEN    # frps 认证token
V2RAY_NAME   # frpc 配置中的块，代理名称 e.g. v2ray
FRP_VMESS_PORT # v2ray 在frps服务中的代理端口
```

打开Actions，执行frp_v2ray.yml，然后修改v2ray客户端的配置，使用`SERVER_ADDR` 和 `FRP_VMESS_PORT`两个值。

每次执行大概有6小时。
