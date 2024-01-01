# websockets

### HTTP VS WBSOCKETS
websockets are full dubplex bidirectional communbication protocol
were as HTTP is cliant and server type 
websockets are long lived where as HTTP connections are terminated for each request
Messages can be sent in either direction at any time and are not transactional in nature
var ws = new WebSocket("wss://normal-website.com/chat");    ----> implementation of websocket WSS protocol is used
the request and response look like JSON

## manipulating WebSocket traffic
to intercept and manipulate wesockets we can use intercept tab of burp proxy which also have websocket history and wensocket tab 
you can also send websocket requests to repeater from websocket history tab

 websocket vulns can leaad to SQLI XXE XSS SSRF etc
 eg --> messgae sent     {"message":"Hello Carlos"}
 rendered message   - -----> <td>Hello Carlos</td>
 so we add payload as     ------> #{"message":"<img src=1 o'nerror='alert(1)'>"}   -----> which can lead to xsss

 Manipulating the WebSocket handshake to exploit vulnerabilities
 X-Forwarded-For: 1.1.1.1   ----> ti bypass ip restictions
