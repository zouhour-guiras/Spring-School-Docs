# Chapter 4: Introduction to the server side 

## <div style="color: Royalblue;"> Table of contents </div>

- Web server definition 
- HTTP / HTTPS protocols 
- HTTP request methods (GET, POST) 

## <div style="color: Royalblue;"> Web server </div>

A web server is a software application or hardware device that serves content to clients over the internet or an intranet using HTTP (Hypertext Transfer Protocol) or its secure variant, HTTPS (HTTP Secure). Web servers are responsible for delivering web pages, files, and other resources requested by clients, typically web browsers.

## <div style="color: Royalblue;"> HTTP / HTTPS protocols  </div>

How do computers communicate with each other?
What languages do they use to communicate with each other? <br>
&rarr; Protocols enable machines to talk to each other.

- Hypertext Transfer Protocol is a client-server communication protocol developed for the World Wide Web. 
- It enables web pages to be exchanged between client and server. HTTPS is the secure variant, using Transport Layer Security protocols.
- **low-level protocols:**<br>
      -  TCP: invented by vint cerf<br>
      -  UDP<br>
- **High- level protocols**: <br>
      - HTTP: HyperText Transfer Protocol<br>
      - HTTPS: Secured HTTP <br>
      - SMTP: send e-mails<br>

**<div style="color: Royalblue;">HTTP protocol basic principle</div>**

![ProtocolHTTP](ProtocolHTTP.png){:style="width:600px;height:250px;"}</br>

**<div style="color: Royalblue;">HTTP protocol: Example</div>**

![HTTP_Example](HTTP_Example.png){:style="width:600px;height:300px;"}</br>

**<div style="color: Royalblue;">Different codes sent with the server response</div>**

- Each HTTP response contains a status code, which is a number indicating whether or not the request was successful.</br>
- There are many possible codes, including the following:</br>
**1XX Information**: The request has not been completed, but is in progress.
**2XX Success**: Query completed successfully.</br>
**3XX Redirection**</br>
**4XX Client-side error**: The client has sent the wrong request</br>
**5XX Server-side error**: The server cannot process the request due to an internal error </br>

- Example:<br>
          **200**: Successful request</br>
          **301 and 302**: redirection, permanent and temporary respectively</br>
          **401**: user not authenticated</br>
          **403**: access denied</br>
          **404**: page not found</br>
          **500 and 503**: server error</br>
          **504**: server did not respond</br>

## <div style="color: Royalblue;">http request methods</div>

- The existing methods are: GET, HEAD, POST, PUT, DELETE, PATCH, OPTIONS, CONNECT, TRACE<br>
**GET**: Request to retrieve data, must not modify anything on the server side<br>
**POST**: Sends data to a server, e.g. to add an item to a shopping cart<br>
**PUT**: Adds or replaces a resource on the server.<br>

&rarr; The difference with POST is that a PUT request is idempotent: calling it once or several times in succession will have the same effect, whereas several POST requests could have side effects, such as placing an item several times in a shopping cart.<br>
**<div style="margin-left: 20px;">DELETE**: Delete a resource</div>
**<div style="margin-left: 20px;">PATCH**: Modify only part of a resource, unlike PUT, which sends the complete representation of the resource to be modified</div>

&rarr;HTTP responses can contain just about anything (file, streamed content, html, css, javascript, json, etc.).

**<div style="color: Royalblue;">IP address Vs host names</div>**


**IP address:**<br>
- Every computer has an address. This is called an IP address.<br>
- It's a sequence of numbers like 205.89.177.26.<br>
- It can be seen as a kind of telephone number.<br>
- So, in theory, you can go to a website by typing the server's address directly into your address bar.<br>


**Host names and DNS:**<br>
- DNS stands for 'Domain Name System'. It translates host names into IP addresses.<br>
- The DNS server acts like a directory consulted by a computer when accessing another computer on a network.<br>
- In other words, the DNS server is the service that associates an IP address with a web site (or a connected computer or server), just as a telephone directory associates a telephone number with a subscriber's name.<br>

**<div style="color: Royalblue;">Anatomy of an HTTP GET request</div>**

![Anatomie](Anatomie.png){:style="width:600px;height:250px;"}</br>

**<div style="color: Royalblue;">Anatomy of an HTTP POST request</div>**

![AnatomiePost](AnatomiePost.png){:style="width:600px;height:250px;"}</br>

**<div style="color: Royalblue;">Anatomy of an HTTP GET response</div>**
![ReponseGET](ReponseGET.png){:style="width:600px;height:250px;"}</br>

- Some queries may also contain a body, i.e. data such as files, or query elements too large to be contained in the query part of the request.

- The methods used to transmit a body are: POST, PUT, DELETE, PATCH

- When a request contains a body, the Content-Type header is used to define the type of request.

- A POST request is generally sent from an HTML form, and causes a change on the server.

- When a form is sent, several body formats may appear:</br>
**application/x-www-form-urlencoded**: series of keys=values separated by '&'.</br>
**multipart/form-data**: each value is sent as a block of data, with a delimiter separating each part </br>
**application/json**: the form is sent as a json {"key1": "value1", "key2": "value2"}.</br>

- The body type depends strongly on the type of data sent.

**<div style="color: Royalblue;">The browser (client)</div>**

- In an HTTP request, the browser is the client.
- The browser makes HTTP requests at several points in the life cycle of a web page:
- When the page first loads, when the user enters the site URL
- When the HTML contains script, css, image or equivalent tags that need to be retrieved.
- When the user clicks on a link and changes page </br>
![Browser](Browser.png){:style="width:600px;height:250px;"}</br>

**<div style="color: Royalblue;">Web page life cycle</div>**
![LifeCycle](LifeCycle.png){:style="width:600px;height:500px;"}</br>

