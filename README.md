# VS_2_Mini_Test

1. a)
The Request-Line begins with a method token, followed by the Request-URI and the protocol version, and ending with CRLF. The elements are separated by SP characters. No CR or LF is allowed except in the final CRLF sequence.

        Request-Line   = Method SP Request-URI SP HTTP-Version CRLF
   
   b)
GET http://192.168.1.1:8080 HTTP/1.1 CRLF ??? not sure about the CRLF

   c)
statelessness and cacheability (or uniform interface not sure)

2. a) 
Socket and ServerSocket
ServerSocket instantiation is what sets up the server to listen at the given port. The server is automatically set up at the computer on which it is run. Socket instantiation uses the accept() method of ServerSocket. This method waits until a client attempts to connect to the server, and it returns an instance of the Socket class. This Socket instance (skt) is now the "warp tunnel" through which one can communicate with the client. A connection to the server by the client is attempted through an instantiation of the Socket class. It attempts to contact the server through the same port where the server is listening. Once a connection is established Client and Server can communicate via input- and outputstreams.

   b)
