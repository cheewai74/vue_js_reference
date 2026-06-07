```
1. Create backend folder
2. npm init -y
3. Create src folder and create a file 'server.js'
4. npm install express
5. npm install --save-dev @babel/core @babel/node @babel/preset-env @babel/cli @babel/plugin-transform-runtime
6. npm install @babel/runtime
7. Create a .babelrc file inside src folder
8. npx babel-node src/server.js
```

src folder:</BR>
```
1. server.js
2. .babelrc
```

.balelrc file:</BR>
```
{
    "presets": ["@babel/preset-env"],
    "plugins": [
        ["@babel/plugin-transform-runtime",{
            "regenerator": true
        }]
    ]
}
```

server.js:</BR>
```
import express from "express";

const app = express();

app.get("/hello", (req, res) => {
  res.send("Hello!");
});

app.listen(8000, () => {
  console.log("Server is listening on port 8000");
});
```
