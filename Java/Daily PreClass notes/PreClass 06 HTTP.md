[Review: High-level HTTP](https://dev.to/dangolant/things-i-brushed-up-on-this-week-the-http-request-lifecycle-)

1.  What are the five steps in the HTTP Request Lifecycle?
	1. **Step 1: Local Processing**
	2.  **Step 2: Resolve an IP**
	3.  **Step 3: Establish a TCP Connection**
	4.  **Step 4: Send an HTTP Request**
	5.  **Step 5: Tearing Down and Cleaning Up**
2.  What are the two things the client needs before it can make an HTTP Request?
	3. hostname for the request
		1.IP address
3.  Explain the three way handshake and what it does.
	1. known as the THREE way handshake 
		1. 1.  The client initiates the active open by sending a `SYN`[7](https://dev.to/dangolant/things-i-brushed-up-on-this-week-the-http-request-lifecycle-#fn7) "control"[8](https://dev.to/dangolant/things-i-brushed-up-on-this-week-the-http-request-lifecycle-#fn8) packet to the server. The client sets the _sequence number_ for the first packet to a random value purposely, in service of security. We’ll refer to this number as `x` for now.
		2.  The server responds with a `SYN-ACK`[9](https://dev.to/dangolant/things-i-brushed-up-on-this-week-the-http-request-lifecycle-#fn9) message, which contains an _acknowledgement number_ for the original message that is always `x+1`, and a new sequence number for the response itself, which is another random number `y`.
		3.  In the third step, the client sends an `ACK`[10](https://dev.to/dangolant/things-i-brushed-up-on-this-week-the-http-request-lifecycle-#fn10) message back to the server with a sequence number equal to `x+1`, which should match the `SYN-ACK` message’s acknowledgment number and ensure that our data is being delivered reliably. The `ACK` message’s acknowledgment number (since it is _acknowledging_ the `SYN-ACK`) is set to one more than the received sequence number, or `y+1`.

[Java HTTP Request example](https://www.baeldung.com/java-http-request)

1.  True or False: When making an HTTP request, you MUST follow any redirect returned by the request. Back up your answer.
	1. True Java, when making an HTTP request, by default, the Java HttpURLConnection class will follow redirects up to a maximum of 20.
2.  Which built-in Java class can be used to perform an HTTP request?
	1. java.net.HttpURLConnection

import java.net.*;
import java.io.*;

public class HttpExample {
    public static void main(String[] args) throws Exception {
        URL url = new URL("http://www.example.com");
        HttpURLConnection con = (HttpURLConnection) url.openConnection();
        con.setRequestMethod("GET");
        int responseCode = con.getResponseCode();
        BufferedReader in = new BufferedReader(new InputStreamReader(con.getInputStream()));
        String inputLine;
        StringBuffer response = new StringBuffer();
        while ((inputLine = in.readLine()) != null) {
            response.append(inputLine);
        }
        in.close();
        System.out.println(response.toString());
    }
}


3.  What HTTP status codes represent a successful response? A redirect? A client error?
	1. -   **Successful response**: Status codes in the 2xx range indicate a successful response. Some examples include:
    
    -   200 OK: The request was successful and the response body contains the requested data.
    -   201 Created: The request was successful and a new resource was created as a result.
    -   204 No Content: The request was successful, but there is no response body.
	-   **Redirection**: Status codes in the 3xx range indicate a redirection. Some examples include:
    
	    -   301 Moved Permanently: The requested resource has been permanently moved to a new URL. The client should update its bookmarks and links to use the new URL.
	    -   302 Found: The requested resource has been temporarily moved to a new URL. The client should continue to use the original URL for future requests.
	    -   307 Temporary Redirect: The requested resource has been temporarily moved to a new URL. The client should continue to use the original URL for future requests.
	-   **Client error**: Status codes in the 4xx range indicate a client error. Some examples include:
    
	    -   400 Bad Request: The request was malformed and could not be processed.
	    -   401 Unauthorized: The client is not authorized to access the requested resource. This typically means that the client needs to provide valid credentials (e.g., a username and password).
	    -   404 Not Found: The requested resource could not be found on the server.