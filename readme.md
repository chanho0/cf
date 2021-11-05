argo

test
```
cloudflared tunnel --hostname <hostname> --url localhost:port
```
config.yml
```
tunnel: xxx
credentials-file: /root/.cloudflared/xxx.json
 
ingress:
  - hostname: <hostname>
    service: http://localhost:port
  - service: http_status:404
```
use
```
cloudflared service install
service cloudflared start
```
