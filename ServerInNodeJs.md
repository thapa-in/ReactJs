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
> Open Terminal and type following command to sart server
```
node http
```
> Go to browser and type in address bar
```
localhost:4100
```
>and press enter

**2. When we have applied changes in server file**
> After made changes we have to close server by press Ctrl+C
> And then strat server by following command
```
node http
```

