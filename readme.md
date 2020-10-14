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

### Questions

### Learnings

### Feature Requests
- 051920[P3]: Use the builtin LED as a crude indicator (packet send, receive, etc.)
 
### Revisions
- 101220
	- new code based branched from cub2bed_client
	- messaging via 900mhz radio removed
	- messaging via MQTT topic added