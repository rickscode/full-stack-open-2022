title 0.5: Single Page App

Client->Server: Authentication Request
Server-->Client: HTTP GET https://studies.cs.helsinki.fi/exampleapp/spa

note over Server:
200 Response Code
end note 

Server-->Client: Return HTML-code
Client->Server:  HTTP GET https://studies.cs.helsinki.fi/exampleapp/main.css

note over Server:
304 Response Code 
(Not Modified client redirection)
end note

Server-->Client: Return main.css
Client->Server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/spa.js

note over Server:
304 Response Code 
(Not Modified client redirection)
end note

Server-->Client: Return spa.js

note over Client:
Browser executs JS code and requests 
JSON file data from server 
end note

Client->Server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/data.json

note over Server:
304 Response Code 
(Not Modified client redirection)
end note

Server-->Client: Return data.JSON [{ content: "HTML is easy", date: "2019-05-23" }, ...]

note over Client:
Browser executes the event handler callback
that renders notes to display 
end note


note over Client:
Notes are displayed in <ul> 
<li> note </>
</ul>
format
end note



