The five steps in the HTTP Request Lifecycle are:

DNS Resolution: The client resolves the domain name to an IP address using DNS.
TCP Connection: The client establishes a TCP connection with the server on the specified port (usually port 80 for HTTP and port 443 for HTTPS).
HTTP Request: The client sends an HTTP request to the server, including the HTTP method (GET, POST, etc.), headers, and optional body.
Server Processing: The server receives the request, processes it, and generates an appropriate response.
HTTP Response: The server sends back an HTTP response to the client, including the response status, headers, and optional body.
2. What are the two things the client needs before it can make an HTTP Request?
The client needs two things before making an HTTP Request:

Server Address (URL): The URL of the server to which the request should be sent.
HTTP Method: The HTTP method to be used in the request, such as GET, POST, PUT, DELETE, etc.
3. Explain the four-way handshake and what it does.
The "four-way handshake" typically refers to the process of establishing and terminating a TCP connection. It involves a series of steps between the client and the server:

Client Sends SYN: The client sends a TCP packet with the SYN (synchronize) flag set to the server.
Server Sends SYN-ACK: The server receives the SYN packet, sends a TCP packet back with the SYN and ACK (acknowledgment) flags set.
Client Sends ACK: The client acknowledges the server's response by sending a TCP packet with the ACK flag set.
Connection Established: The TCP connection is now established and data can be exchanged.
For termination:

Client Sends FIN: The client initiates connection termination by sending a TCP packet with the FIN (finish) flag set.
Server Sends ACK: The server acknowledges the client's FIN packet.
Server Sends FIN: The server also initiates termination by sending a TCP packet with the FIN flag set.
Client Sends ACK: The client acknowledges the server's FIN packet, completing the termination process.
4. True or False: When making an HTTP request, you MUST follow any redirect returned by the request. Back up your answer.
True. When making an HTTP request, if the server responds with a redirect (status codes 3xx), the client is expected to follow the redirect by sending another request to the new URL provided in the redirect response. This is specified by the HTTP protocol and ensures that clients are directed to the correct resource.

5. Which built-in Java class can be used to perform an HTTP request?
The built-in Java class that can be used to perform an HTTP request is HttpURLConnection. This class provides a way to establish a connection to an HTTP server, send an HTTP request, and receive an HTTP response.

6. What HTTP status codes represent a successful response? A redirect? A client error?

Successful Response (2xx): Status codes in the 200 range represent successful responses. For example, status code 200 indicates a successful GET request.
Redirect (3xx): Status codes in the 300 range indicate redirects. Examples include 301 (Moved Permanently), 302 (Found), and 307 (Temporary Redirect).
Client Error (4xx): Status codes in the 400 range indicate client errors. For example, 404 (Not Found) and 400 (Bad Request) are common client error codes.