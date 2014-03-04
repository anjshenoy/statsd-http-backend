statsd-http-backend
===================

POST Data to a HTTP Backend

installation
============

   npm install statsd-http-backend

usage
=====

In config.js:  

```
{
backends: [ "statsd-http-backend" ],
hostname: "hostname.where.deployed"
bridgeURL: "http://yourdomain.that.eats.this.post"
}
```

notes
=====

Submits a POST to any domain that the bridgeURL exposes. Hostname is
optional. If specified, it gets added to the URL as a query param like
so:


```
http://yourdomain.that.eats.this.post?hostname=myhost.name.com
```
