# Inko TLS
This is an Inko package that provides a wrapper around `TcpClient` to allow for TLS communication (https/wss)

## Examples
```js
import tls(TLSSocket)

let client = TcpClient.new(ip, port).get
let sock = TLSSocket.new(client)
```
You can then use `sock.write_bytes` or `sock.write_string` and get a response with `sock.read`.

## 

You can easily integrate inko-tls with [inko-requests](https://github.com/fres621/inko-requests) and [inko-ws](https://github.com/fres621/inko-ws).