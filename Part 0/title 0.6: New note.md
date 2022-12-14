title 0.6: New note

Client->Server: HTTP POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa

note over Server:
POST new note to address /new_note_spa 
in JSON type format
end note 

note over Server:
201 Response Code
end note 

Server-->Client: Server responds with new updated JSON data

note over Client:
Browser executes JS code function redrawNotes()
and dynamically displays new notes 
without NY URL redirects or reloads
end note
