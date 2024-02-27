# Chapter 1 : An introduction to the web


## <div style="color: Royalblue;"> Table of contents </div>

- History of the web
- Client-server architecture
- Static vs dynamic web
- The difference between front-end and back-end 
- Website editors and frameworks

## <div style="color: Royalblue;"> The Web: what you need to know! </div>


![what you need to know!](What_you_need_to_know.png){:style="width:700px;height:300px;:class="centered-image"}

## <div style="color: Royalblue;"> A little bit of history… </div>

![A little bit of history](little_history.png){:style="width:800px;height:300px;"}

![A little bit of history](history2.png){:style="width:800px;height:300px;"}

##### <div style="color: Royalblue;"> What is the Internet? </div>

![Internet](Internet.png){:style="width:500px;height:200px;"}

A global computer network consisting of a set of national, regional and private networks (networks of networks), which are linked by the TCP/IP communication protocol and which work together to provide a unique interface to their users.

**TCP/IP communication protocol:** 
**(Transmission Control Protocol/Internet Protocol)**
Is a set of rules used to enable communication between devices on a computer network. It is widely used as a communications protocol on the Internet, and is also used in many local area networks (LANs) and corporate networks.

##### <div style="color: Royalblue;"> Network & Computer network </div>

![network_computer](network_computer.png){:style="width:700px;height:300px;"}

##### <div style="color: Royalblue;"> Communication protocol & TCP/IP suite </div>
![communication_protocol](communication_protocol.png){:style="width:800px;height:300px;"}

##### <div style="color: Royalblue;"> The key players of the Internet </div>

![key_players](key_players.png){:style="width:900px;height:350px;"}

##### <div style="color: Royalblue;"> Some examples of Internet protocols </div>

![example_protocols](example_protocols.png){:style="width:800px;height:300px;"}

##### <div style="color: Royalblue;"> Internet services </div>

![internet_service](internet_service.png){:style="width:600px;height:300px;"}

##### <div style="color: Royalblue;"> World Wide Web (WWW) </div>

![WWW](WWW.png){:style="width:800px;height:300px;"}

##### <div style="color: Royalblue;"> Web evolution </div>

![Web_evolution](web_evolution.png){:style="width:900px;height:400px;"}

##### <div style="color: Royalblue;"> How does the Web work? </div>

![Web_Work](Web_Work.png){:style="width:700px;height:300px;"}

##### <div style="color: Royalblue;"> Web servers </div>

![Web_service](Web_service.png){:style="width:700px;height:300px;"}

![Web_server_2](web_server_2.png){:style="width:700px;height:300px;"}

➔ A program can be both server and client of other servers.<br>
➔ retrieving a web page that contains information from a database <br>

![Web_server3](web_server3.png){:style="width:600px;height:300px;"}

## <div style="color: Royalblue;"> Client / Server </div>

![Client_Server](Client_Server.png){:style="width:700px;height:300px;"}

• The DNS (Domain Name System) protocol allow to match an IP address with a name in order to avoid to retain IP addresses.<br>
Exemple : 195.83.142.250 ➔

![DNS](DNS.png){:style="width:600px;height:300px;"}

• The FQDN allows access to a machine on which a number of resources
are available and which are served by different protocols.<br>
• A URL (Uniform Resource Location) allows to specify which resources
to reach, and with which protocol.

![Client_Server2.png](Client_Server2.png){:style="width:600px;height:200px;"}

## <div style="color: Royalblue;"> Static vs dynamic web </div>

### <div style="color: Royalblue;"> A static WEB page </div>

• Visible as designed<br>
• Can present different forms of content: images, flash animations, video, music, etc.<br>
• Its content does not change => Static <br>
• Stored in the Web server which only displays it when requested <br>
• The entire code that composes it is interpreted directly by the client (Web
browser) <br>

![Static_Web](Static_Web.png){:style="width:600px;height:200px;"}

##### <div style="color: Royalblue;"> Composition of a web page </div>

![page_content](page_content.png){:style="width:600px;height:300px;"}

![Web_page_js](Web_page_js.png){:style="width:600px;height:300px;"}

##### <div style="color: Royalblue;"> Example of a web page managing a CV-library </div>

![CV_sympsons](CV_sympsons.png){:style="width:800px;height:400px;"}

![Example_CV](Example_CV.png){:style="width:800px;height:400px;"}

• <span style="color:red;"> File:// </span> : local protocol <br>
             - Files must be accessible on the machine used to view them <br>
             - Files are not served by a web server <br>
• <span style="color:red;"> http:// </span>: client-server protocol <br>
             - Files are retrieved from the web server machine to the client
machine (web browser) <br>
             - Files are served by a server usually on another machine <br>

<span style="color:red;"> Rq </span> :(firefox et chrome) :<span style="color:red;">[ctrl]+[maj]+i </span> gives access to a tool panel allowing
to visualize the network exchanges

![tool_panel](tool_panel.png){:style="width:500px;height:200px;"}

##### <div style="color: Royalblue;"> Static Web: advantages and disadvantages</div>

![avantage_desavantage_static_web](avantage_desavantage_static_web.png){:style="width:600px;height:300px;"}

### <div style="color: Royalblue;"> A dynamic web page </div>

![dynamic_page](dynamic_page.png){:style="width:700px;height:300px;"}

![Dynamic_web_2](Dynamic_web_2.png){:style="width:700px;height:300px;"}

![dynamic_web_3](dynamic_web_3.png){:style="width:800px;height:500px;"}

##### <div style="color: Royalblue;"> Dynamic Web site: advantages </div>

![Avantage_dynamic_web](Avantage_dynamic_web.png){:style="width:600px;height:400px;"}

##### <div style="color: Royalblue;"> Dynamic Web site: disadvantages </div>

![disavantage_dynamic_web](disavantage_dynamic_web.png){:style="width:700px;height:300px;"}

## <div style="color: Royalblue;"> The difference between front-end and back-end </div>

![FrontEnd_Backend](FrontEnd_Backend.png){:style="width:700px;height:400px;"}

##### <div style="color: Royalblue;"> The Back-end: its competences </div>

The Back-End is divided into three essential parts: <br>
**Server (or web hosting)**: seen as a hard disk accessible 24 hours a day, on which the pages of the website are stored.<br>
**Databases**: comparable to a large table with columns containing the necessary
information on which the development is based, for example "name", "first name",
"password", "current purchase".<br>
**Dynamic programming languages**: allow to keep, process, modify data and provide updated information on a website (such as news, product sheets, images, videos, etc.).
The most used languages are PHP, Ruby, Python, SQL <br>
**Frameworks**: to make the code clearer, easier to modify and simpler to maintain as a team, for example: CakePHP, Symphony

## <div style="color: Royalblue;"> Website editors and frameworks </div>

##### <div style="color: Royalblue;"> Website editors </div>

![WebsiteEditors](WebsiteEditors.png){:style="width:900px;height:350px;"}

##### <div style="color: Royalblue;"> Some examples </div>

![example_editors](example_editors.png){:style="width:600px;height:300px;"}

![Webeditor2](Webeditor2.png){:style="width:600px;height:300px;"}

##### <div style="color: Royalblue;"> Frameworks </div>

![Frameworks](Frameworks.png){:style="width:600px;height:300px;"}

## <div style="color: Royalblue;"> Content Management System (CMS) </div>

![ContentManagementSystem](ContentManagementSystem.png){:style="width:700px;height:300px;"}

##### <div style="color: Royalblue;"> Content Management System (Some examples) </div>

![CMS_examples](CMS_examples.png){:style="width:700px;height:300px;"}

##### <div style="color: Royalblue;"> Content Management System (Useful links) </div>

![CMS_UsefulLinks](CMS_UsefulLinks.png){:style="width:700px;height:300px;"}
