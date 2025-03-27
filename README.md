> [!IMPORTANT]  
> As of 27/03/25, inko-tls has been discontinued.
>
> TLS client support is now available in Inko's standard library
>
> For more information refer to [inko docs / std.net.tls](https://docs.inko-lang.org/std/main/module/std/net/tls/)

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
