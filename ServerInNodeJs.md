**1. How to Create Server**
 > Create http name file (we can choose any name for this file)
```
const http= require('http');

const server = http.createServer((req, resp)=>{
    resp.write('Welcome');
    resp.end();
})

server.listen(4100);
```
> Go to browser and type in address bar
```
localhost:4100
```
>and press enter


