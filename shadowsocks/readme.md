# ss

### 使用

```bash
# 安装 docker 和 docker-compose
# 创建自定义配置文件
cp config.json.example config.json
# 编辑自定义配置 config.json ，然后执行：
docker-compose up -d --build
```

```text
// config.json
{
    "server": "*.*.*.*",      --- 填写“私有”IP
    "server_port": **,        --- 自定义对外端口
    "local_address": "127.0.0.1",
    "local_port": 1080,
    "password": "****",       --- 密码
    "timeout": 300,           --- 超时时间
    "method": "aes-256-cfb",  --- 加密方式
    "fast_open": false        --- 要开启需要服务端和客户端都是 linux 3.7+,不确定就设置为false
}
```