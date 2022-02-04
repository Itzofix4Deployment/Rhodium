<h1>Rhodium<h2>Fast, Light, Capable.</h2><h3>Successor to <a target="_blank" href="https://github.com/ludicrousdevelopment/palladium">Palladium</a><h3>Secondary Proxy to <a target="_blank" href="https://github.com/titaniumnetwork-dev/corrosion">Corrosion</a> and <a target="_blank" href="https://github.com/binary-person/womginx">Womginx</a></h1>

`index.js`
```js
var req=require,
  server=req("http").Server(),
  proxy=new(req("./"))({title:"Rhodium",server:server});proxy.init();server.on("request",(e,r)=>(e.url.startsWith(proxy.prefix)?proxy.request(e,r):r.end(req("fs").readFileSync("./index.html")))).listen(80);
```

`config`
```json
{
  "userAgent": "fx", // Firefox userAgent Spoof
  "prefix": "/service/", // Proxy Prefix
  "wss": true, // WebSocket Server
  "corrosion": [false, {}], // Corrosion Dual-Server
  "title": "Rhodium", // Page Title on Proxied Pages
  "server": http.Server() // Your Http Server
}
```
[userAgent](#userAgent)

[prefix](#prefix)

[wss](#wss)

[corrosion](#corrosion)

[title](#title)

[server](#server)

<div id="server">HELLO WHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWvv</div>

<div id="wss">HELLO WHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWWHBFHKEHFKEBTGUYEFHYEFNYHEFINHYEWGYEQFUJEQHFUHEQFYEWDAYFHNEWHFJGYHEWGNJHWEBGJYHEWGYUJHEWvv</div>