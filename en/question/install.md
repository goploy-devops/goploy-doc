# Installation problem

# Pattern dist: no matching files found

```bash
cd ./web
npm install
npm run build
```

# Error during Websocket handshake

The reason is that the reverse proxy settings are incorrect
```nginx
proxy_set_header Upgrade         $http_upgrade;
proxy_set_header Connection      "upgrade";
```

# Illegal request

Please check if the reverse proxy is correct, check if it has cookies