# cub2bed_server
## What is cub2bed_server? 
Simple two-way message appliance

### Purpose
Client message appliance alerts server appliance of message and receives status updates from server

### Contributors

### Software Dependencies not in Arduino Library Manager

### BOM
- 1x: Adafruit Feather Huzzah 8266 https://www.adafruit.com/product/2471
- 1X: NeoPixel
- 2x: button
- 1 protoboard
- wire

### Pinouts
- see Fritzing diagram

### Information Sources

### Issues
- 051920[P2]; implement robust error handling; how does the user know what state they are in (visually, programmatically)
- 071620[P2]; need to step up 3.3v to 5v for the button LED
- 101220[P3]; AdafruitIO feeds not setup properly
- 101520[P1]; If cub2bedPub fails, downstream is not handled properly
- 101520[P2]; statusLightPub Off should be handled by c2b client, not server, ensuring light only goes on when the client has recognized cub2bed message from server

### Questions

### Learnings

### Feature Requests
- 051920[P3]: Use the builtin LED as a crude indicator (packet send, receive, etc.)
- 101220[P2]; MQTT QoS 1
 
### Revisions
- 101220
	- new code branched from cub2bed_client
	- messaging via 900mhz radio removed
	- messaging via MQTT topic added
- 101520
	- MQTT code improvements