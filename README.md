# Aplestro Tunnel

Your way in Aplestro ecosystem

Aplestro Tunnel exposes your localhost to the Aplestro for easy testing and sharing! No need to mess with DNS or deploy just to have others test out your changes.

Based on <a href="https://localtunnel.github.io/www/">Localtunnel</a>

## use ##

```
npm i
```

You need to add your app to Aplestro. You should check "Use Aplestro tunnel". In URL you should enter your relative endpoint of your app (or don't enter if your endpoint is the root).

![](http://about.aplestro.com/content/new-app2-tunnel.png)

You need to obtain "App ID" and "Tunnel Key". 

![](http://about.aplestro.com/content/new-app2-tunnel-in-list.png)

Assuming your local server is running on port 3333. 

```
node bin/client -p 3333 -s 123example_YourAppId -x 321example_TunnelKey
```

It will connect to the tunnel server, setup the tunnel, and tell you what url to use for your app. 
Your url will be https:// <YourAppId> .tunnel.aplestro.com. This url is saved for your application forever.
You are ready to open your app in Aplestro by "URL in Aplestro".

### arguments

* `-p` port
* `-s` your App ID
* `-x` tunnel key

## License ##
MIT
