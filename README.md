# part-0

Excercise 0.4 new-note


browser->server: HTTP POST https://studies.cs.helsinki.fi/exampleapp/new-notes
server->browser: status code

note over server:
server sent a status code to
the browser that redirects the
browser to reload the  html code,notes page

browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/notes
server-->browser: HTML-code
browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/main.css
server-->browser: main.css
browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/main.js
server-->browser: main.js

note over browser:
browser starts executing js-code
that requests JSON data from server 


browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/data.json
server-->browser: [{ content: "HTML is easy", date: "2019-05-23" }, ...]

note over browser:
browser executes the event handler
that renders notes to display




Excercise 0.5 spa


browser->server:  HTTP GET https:// studies.cs.helsinki.fi/exampleapp/spa

server->browser: HTML-code

browser->server: HTTP GET  HTTP GET https:// studies.cs.helsinki.fi/exampleapp/spa

server->browser: main.css

browser->server:  HTTP GET https:// studies.cs.helsinki.fi/exampleapp/spa.js

server->browser: spa.js

notes over browser:

The contents of the HTML page are

 manipulated with JavaScript that 

executes in the browser.





Excercise 0.6 spa-new-note

browser->server: GET HTTP https://studies.cs.helsinki.fi/exampleapp/spa_new_note

note over browser:

content-type:application/json

{content: "test2",date: "------------"}

server->browser:  201 created

note over browser:

browser executes the event handler that

renders notes to display

