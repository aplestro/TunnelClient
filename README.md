# Aplestro Tunnel

Your way in Aplestro ecosystem

Aplestro Tunnel exposes your localhost to the Aplestro for easy testing and sharing! No need to mess with DNS or deploy just to have others test out your changes.

Based on <a href="https://localtunnel.github.io/www/">Localtunnel</a>

## use ##

```
npm i
```

You need to add your app to Aplestro. You need to obtain "YourAppId" and "TunnelKey"

Assuming your local server is running on port 3333. 

```
node bin/client -p 3333 -s 123example_YourAppId -x 321example_TunnelKey
```

It will connect to the tunnel server, setup the tunnel, and tell you what url to use for your app. 
Your url will be https://YourAppId.tunnel.aplestro.com. This url is saved for your application forever.
You a ready to work in Aplestro.

### arguments

Below are some common arguments. See `lt --help` for additional arguments

* `-p` port
* `-s` request a your public AppId
* `-x` tunnel key

## License ##
MIT
