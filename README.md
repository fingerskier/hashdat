# hashdat
Automagically synchronized remote data

## Process
* Authenticate
  * Client receives a code
* Client opens a web-socket connection
  * access to a data-structure is via hash of the URL using the aforementioned code
* Updates
  * Data-diff = {hash-name, timestamp, changes}
    * changes = {thing1:val, thing2:val, ...}
  * Client cycle
    * Data-diff since last update is sent to the server
  * Server cycle
    * ..._as opposed to shipping change-ops to be played back...
    * this necessitates reasonably sized data packages
    * perhaps provide a facility to smoothly transition between current and server states for some environs
* Storage
  * DHT
  
  
## Implementation
H(hashField)`OP${data}`
