# Week 14 Homework: Web Development
I'm still a newbie in Github but hopefully this README.md is readable and understandable. I copy the questions from Gitlabs and should be readable as well. This are some mispelled words through out this file so lookout for it. 

## Questions 
### HTTP Requests and Responses

1. What type of architecture does the HTTP request and response process occur in? 

        Client-Server Architecture since the requests connected to form client to server and then send responses back to the client 

2. What are the different parts of an HTTP request?

        Request Line, Headers, and Body

3. Which part of an HTTP request is optional?

        Request Body is optional

4. What are the three parts of an HTTP response?

        Headers, Status Line, and Response Body

5. Which number class of status codes represents errors?

        There are 400 codes that indicate client errors which means the webpage does not exits or cannot be accessed. 

6. What are the two most common request methods that a security professional will encounter?

        GET & POST requests are the most common request methods that a security professional will encounter. 

7. Which type of HTTP request method is used for sending data?

        POST request is used for sending data. 
        
8. Which part of an HTTP request contains the data being sent to the server?

        Request body contains the data being sent to the server.

9. In which part of an HTTP response does the browser receive the web code to generate and style a web page?

        Response body does the browser receive the web code to generate and style a web page.

### Using Curl 

10. What are the advantages of using curl over the browser?
    
    * It can manage HTTP Requests/Response in a repetative way. 
    * It can verify servers respond to certain requests/methods. 
    * It search for vulnerabilities. 
    * It ultilzie grep or output it in files. 

11. Which curl option is used to change the request method? 
   * -X can use different method. 

12. Which curl option is used to set request headers?

  * -H sets request header. 


13. Which curl option is used to view the response header?

  * -I which filter to view the reponse headers only. 


14. Which request method might an attacker use to figure out which HTTP requests an HTTP server will accept?

  * GET request because attacker could requests data from a server to figure out which HTTP requests that an HTTP server server will accept.
  * Options is another request method that the attacker might figure out since it lists out the communication options for target resource. 

### Sessions and Cookies 

15. Which response header sends a cookie to the client? 
   
        HTTP/1.1 200 OK
        Content-type: text/html
        Set-Cookie: cart=Bob
        
   * The set-cookie sends the cookie to the client, which the cookie sent in cart=Bob. 
      
16. Which request header will continue the client's session?

        GET /cart HTTP/1.1
        Host: www.example.org
        Cookie: cart=Bob
   * The cookie will continue the client's session. 
        
### Example HTTP Requests and Responses 
    
#### HTTP Request 

    POST /login.php HTTP/1.1
    Host: example.com
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Content-Type: application/x-www-form-urlencoded
    Content-Length: 34
    Upgrade-Insecure-Requests: 1
    User-Agent: Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N) AppleWebKit/537.36 (KHTML, like Gecko)
    Chrome/80.0.3987.132 Mobile Safari/537.36
    
    username=Barbara&password=password
    
17. What is the request method? 

  * Post 


18. Which header expresses the client's preference for an encrypted response?

  * Upgrade-Insecure-Requests: 1


19. Does the request have a user session associated with it?

  * Session is not restablished yet 


20. What kind of data is being sent from this request body?

  *  Login


#### HTTP Response 
    
    HTTP/1.1 200 OK
    Date: Mon, 16 Mar 2020 17:05:43 GMT
    Last-Modified: Sat, 01 Feb 2020 00:00:00 GMT
    Content-Encoding: gzip
    Expires: Fri, 01 May 2020 00:00:00 GMT
    Server: Apache
    Set-Cookie: SessionID=5
    Content-Type: text/html; charset=UTF-8
    Strict-Transport-Security: max-age=31536000; includeSubDomains
    X-Content-Type: NoSniff
    X-Frame-Options: DENY
    X-XSS-Protection: 1; mode=block

    [page content]
21. What is the response status code? 

   * 200

22. What web server is handling this HTTP response?

   * Apache

23. Does this response have a user session associated to it?

   * Yes, the SessionID=5

24. What kind of content is likely to be in the [page content] response body?

   * Text code


25. If your class covered security headers, what security request headers have been included?

   * XSS protection or Strict Transport Security 

### Monoliths and Microservices 

26. What are the individual components of microservices called?

   * Services 


27. What is a service that writes to a database and communicates to other services?

   * API services 

28. What type of underlying technology allows for microservices to become scalable and have redundancy?

   * Containers & load balancer

### Deploying and Testing a Container Set

29. What tool can be used to deploy multiple containers at once?

   * Docker

30. What kind of file format is required for us to deploy a container set?

   * .yml files 

### Databases 

31. Which type of SQL query would we use to see all of the information within a table called customers?

   * SELECT column_name FROM customers

32. Which type of SQL query would we use to enter new data into a table? (You don't need a full query, just the first part of the statement.)

   * INSERT INTO table_name (column1, etc.) VALUES (value1, etc.); 

33. Why would we never run DELETE FROM <table-name>; by itself?

   * It deletes the entire table since it does not have the select statement.  

No bonus this time :(
  


