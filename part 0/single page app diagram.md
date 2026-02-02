```mermaid
sequenceDiagram
    participant browser
    participant server

     browser ->> server: GET https://studies.cs.helsinki.fi/exampleapp/spa
    activate server
    server -->> browser: HTML document
    deactivate server

Note right of browser: only one request sent to the server which renders the html document to the browser
```