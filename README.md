# beeline-proxy

Proxy web app with static to dev port

1. Forward 80 port from nginx-controller pod (sudo!)
2. Install [mkcert](https://github.com/FiloSottile/mkcert) for making locally-trusted development certificates. 
3. Run mkcert

    ```
    mkcert -cert-file cert/cert.crt --key-file cert/key.key university.beeline.uz
    ```

4. Run proxy 
    
    ```
    docker-compose up -d
    ```
5. Adds 127.0.0.1 university.beeline.uz to `/ets/hosts`

