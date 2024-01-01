# websockets

### HTTP VS WBSOCKETS
websockets are full dubplex bidirectional communbication protocol
were as HTTP is cliant and server type 
websockets are long lived where as HTTP connections are terminated for each request
Messages can be sent in either direction at any time and are not transactional in nature
var ws = new WebSocket("wss://normal-website.com/chat");    ----> implementation of websocket WSS protocol is used
the request and response look like JSON

## manipulating WebSocket traffic
