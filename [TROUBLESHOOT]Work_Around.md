```
rmdir /s /q node_modules
del package-lock.json

npm install
set NODE_OPTIONS=--openssl-legacy-provider
npm run serve
```
