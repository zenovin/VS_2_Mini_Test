# VS_2_Mini_Test

1. 

a)
The Request-Line begins with a method token, followed by the Request-URI and the protocol version, and ending with CRLF. The elements are separated by SP characters. No CR or LF is allowed except in the final CRLF sequence.

        Request-Line   = Method SP Request-URI SP HTTP-Version CRLF
   
   b)
GET http://192.168.1.1:8080 HTTP/1.1 CRLF ? not sure about the CRLF

   c)
statelessness and cacheability (or uniform interface not sure ?)


2. 

a) 
Socket and ServerSocket
ServerSocket instantiation is what sets up the server to listen at the given port. The server is automatically set up at the computer on which it is run. Socket instantiation uses the accept() method of ServerSocket. This method waits until a client attempts to connect to the server, and it returns an instance of the Socket class. This Socket instance (skt) is now the "warp tunnel" through which one can communicate with the client. A connection to the server by the client is attempted through an instantiation of the Socket class. It attempts to contact the server through the same port where the server is listening. Once a connection is established Client and Server can communicate via input- and outputstreams.

   b)
Blocking behaviour is when a method blocks the execution of the surrounding program while waiting for something. For example, an InputStream read from a Socket socket will block, rather than returning EOF, until a TCP packet with the FIN flag set is received. It is only the read methods in InputStream that show blocking behaviour.


3. 

a)
false
  
   b)
false

   c)
true ?

   d)
false


4. 

a)
The WSDL File. It can be accessed through the link given in the assignment. ?

   b)
They can be found in here: http://vslab.inf.ethz.ch:8080/SunSPOTWebServices/SunSPOTWebservice?xsd=1

<xs:element name="getSpot" type="tns:getSpot"/>

<xs:element name="getSpotResponse" type="tns:getSpotResponse"/> ?

   c)
One would change the expression after transport in the WSDL file to http://schemas.xmlsoap.org/soap/smtp.

<soap:binding transport="http://schemas.xmlsoap.org/soap/http" style="document"/>

The address would have to be an email-address since SMTP is a mail-protocol.


5.

a)

