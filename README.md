# VS_2_Mini_Test

1. 

a)
The Request-Line begins with a method token, followed by the Request-URI and the protocol version, and ending with CRLF. The elements are separated by SP characters. No CR or LF is allowed except in the final CRLF sequence.

        Request-Line   = Method SP Request-URI SP HTTP-Version CRLF
   
   b)
GET / HTTP/1.1\r\n
Host: 192.168.1.1:8080\r\n\r\n

GET http://192.168.1.1:8080/ HTTP/1.0\r\n\r\n


   c)
statelessness and cacheability ?

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

```
<xs:element name="getSpot" type="tns:getSpot"/>

<xs:complexType name="getSpot">
  <xs:sequence>
    <xs:element name="id" type="xs:string" minOccurs="0"/>
    </xs:sequence>
  </xs:complexType>


<xs:element name="getSpotResponse" type="tns:getSpotResponse"/>

<xs:complexType name="getSpotResponse">
 <xs:sequence>
    <xs:element name="return" type="tns:sunSpot" minOccurs="0"/>
    </xs:sequence>
  </xs:complexType>
```
   c)
One would change the expression after transport in the WSDL file to http://schemas.xmlsoap.org/soap/smtp.

<soap:binding transport="http://schemas.xmlsoap.org/soap/http" style="document"/>

The address would have to be an email-address since SMTP is a mail-protocol.


5.
   a)
10.0.2.15	The emulated device network/ethernet interface
All emulators have their own router. 

   b)
The emulated device loopback interface.
To the emulated device itself.

   c)
10.0.2.2

   d)
To communicate with an emulator instance behind its virtual router, you need to set up network redirection on the virtual router. Clients can then connect to a specified guest port on the router, while the router directs traffic to/from that port to the emulated device host port.
(from https://developer.android.com/studio/run/emulator-networking.html)

