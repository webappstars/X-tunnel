 -block string
        
        客户端拦截 UDP 端口列表，逗号分隔，如 443,8443 (default "443")
  -cert string
        
        TLS证书文件路径（默认:自动生成，仅服务端）
  -cidr string
        
        允许的来源 IP 范围 (CIDR),多个范围用逗号分隔 (default "0.0.0.0/0,::/0")
  -dns string
        
        查询 ECH 公钥所用的 DNS 服务器 (支持 DoH 或 UDP) (default "https://doh.pub/dns-query")
  -ech string
        
        用于查询 ECH 公钥的域名 (default "cloudflare-ech.com")
  -f string
        
        服务地址/代理地址 (客户端模式: wss://host:port | 服务端模式: socks5://[user:pass@]host:port)
  -fallback
        
        是否禁用 ECH 并回落到普通 TLS 1.3 (默认 false)
  -insecure
        
        客户端 wss 模式忽略证书校验
  -ip string
        
        指定解析的IP地址（仅客户端：将 wss 主机名定向到该 IP 连接，多个IP用逗号分隔）
  -ips string
        
        服务端解析目标地址的IP偏好 (仅客户端有效)
         4: 仅IPv4
         6: 仅IPv6
         4,6: IPv4优先
         6,4: IPv6优先
  -key string
        
        TLS密钥文件路径（默认:自动生成，仅服务端）
  -l string
        
        监听地址 (支持多个，用逗号分隔)
        格式示例:
          socks5://[user:pass@]0.0.0.0:1080
          http://[user:pass@]0.0.0.0:8080
          tcp://0.0.0.0:2000/1.2.3.4:22
          ws://0.0.0.0:80/path (服务端模式)
          wss://0.0.0.0:443/path (服务端模式)
  -n int
        
        每个IP建立的WebSocket连接数量 (default 3)
  -token string
        
        身份验证令牌（WebSocket Subprotocol）
