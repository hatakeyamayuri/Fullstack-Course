```mermaid
sequenceDiagram
    participant browser
    participant server

    Note right of browser: The user clicks the Save button

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: [{content: "incredibly confused", date: "2025-03-17T05:55:25.427Z"}]
    deactivate server
```