# dev-proxy
Proxy web app with static to dev port


```
docker-compose up -d
```

Go to http://localhost and the request will be proxied to app port

TODO: add templates

You add statics files to statics/public. I needed to avoid CORS in an iframe and external scripts

```
mkcert -cert-file cert/cert.crt --key-file cert/key.key go.teachbase.local custom.teachbase.local
```
