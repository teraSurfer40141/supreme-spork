```mermaid
sequenceDiagram
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: created
    deactivate server

    Note right of browser: Javascript code automatically adds note to server without reloading it.

```