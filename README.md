# Inko TLS
> [!WARNING]  
> This is a WIP. Some things might not work as described.

This is an Inko package that lets you create TCP sockets with TLS

## Examples
```js
import std.net.ip(IpAddress)
import tls(TLSSocket)

let sock = TLSSocket.new(IpAddress.v4(127, 0, 0, 1), 443)
```
You can then use `sock.write_bytes` or `sock.write_string` and get a response with `sock.read`.

## 

You can easily integrate inko-tls with [inko-requests](https://github.com/fres621/inko-requests) and [inko-ws](https://github.com/fres621/inko-ws).