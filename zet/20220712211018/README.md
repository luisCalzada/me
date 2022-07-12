# What is ASP.Net Core SignalR?
It's an open source library, for ASP.Net Core, that handles real time communication between server and client.
This allows you to call a function on the client side from the server side or the other way around, instead of the traditional
client executes method on server.

SignalR uses *hubs* to communicate between clients and servers. 
It comes with two built-in hub protocols. One text protocol based on JSON and a binry protocol based on MessagePack.
Using MessagePack you get smaller messages but requires browsers to support XHR level 2.

Hubs will send messages with the name of a method and the parameters that said method requires. When the message is received,
the client will try to match the method name to an existing one and if so, it will execute it with the deserialized parameters.

SignalR will handle all of the connection management (keep alive, handshakes, etc).
It can send messages to all connected clients or only to specific clients or 'groups'.
It scales really good.

Supports and chooses the best transport method from: 
* WebSockets
* Server-Sent Events
* Long Polling

  #.NetCore #Microsoft #RealTimeCommunication #WebDev #FullStack
