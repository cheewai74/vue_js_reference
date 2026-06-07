```
1. Create backend folder
2. npm init -y
3. Create src folder and create a file 'server.js'
4. npm install express
5. npm install --save-dev @babel/core @babel/node @babel/preset-env @babel/cli @babel/plugin-transform-runtime
6. npm install @babel/runtime
7. Create a .babelrc file
```

.balelrc file:</BR>
```
{
    "presets": ["@babel/preset-env"],
    "plugin": [
        ["@babel/plugin-transform-runtime",{
            "regenerator": true
        }]
    ]
}
```
