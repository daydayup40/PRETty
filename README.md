# PRETty
"PRinter Exploitation Toolkit" LAN automation tool

![alt text](https://github.com/BusesCanFly/PRETty/blob/master/screenshot.png "Who doesn't love ASCII art?")

PRETty is useful when a large number of printers are present on a network. Instead of scanning, logging, and manually running PRET againt each individual printer, PRETty will automatically discover and run choosen PRET payloads against all printers on the target network.

Additionally, PRETty can be used to automate command/payload delivery to any given list of printers (See the "Lists" section)

# GUIDE:

## Installation
1. Install [PRET](https://github.com/RUB-NDS/PRET) and all required dependencies
2. Install requirements: `sudo pip install termcolor` and `sudo apt -y install netdiscover`
3. Navigate to where you installed [PRET](https://github.com/RUB-NDS/PRET): `cd PRET`
4. Install PRETty into [PRET](https://github.com/RUB-NDS/PRET): `git clone https://github.com/BusesCanFly/PRETty`
5. Navigate to PRETty: `cd PRETty`
6. Make PRETty executable: `chmod +x PRETty.py`
* One line variant (from [PRET](https://github.com/RUB-NDS/PRET) folder): `sudo pip install termcolor && sudo apt -y install netdiscover && git clone https://github.com/BusesCanFly/PRETty && cd PRETty && chmod +x PRETty.py`
* One line variant w/ [PRET](https://github.com/RUB-NDS/PRET) installation: `pip install colorama pysnmp && apt-get install imagemagick ghostscript && git clone https://github.com/RUB-NDS/PRET && cd PRET && sudo pip install termcolor && sudo apt -y install netdiscover && git clone https://github.com/BusesCanFly/PRETty && cd PRETty && chmod +x PRETty.py`

## Lists
* PRETty automatically scans the LAN for HP/Brother/Kyocera printers and creates an IP list for itself
	* However, you can place custom IP lists in `PRETty/IP/`
* PRETty comes with pre-made command files for PRET located in `PRETty/commands/`
	* However, you can place additional command files in `PRETty/commands/`
	
## Usage
1. Run PRETty with `./PRETty.py` and follow the prompts :D

## Disclaimers
### The standard internet fun disclaimer applies. Don't commit crimes, be responsible. 
### I am in no way responsible for anything and everything you do with PRETty.

## Links
PRETty has been seen in:
* https://www.kitploit.com/2019/01/pretty-printer-exploitation-toolkit-lan.html
* https://www.hack4.net/2019/01/pretty-printer-exploitation-toolkit-lan.html
* https://www.reddit.com/r/blackhat/comments/ad7hre/printer_exploitation_toolkit_lan_automation_tool/
* https://twitter.com/netbiosX/status/1081855584260030464
* https://twitter.com/MightyPearMan/status/1082728115531640832
* https://twitter.com/wugeej/status/1082783931248693250
* https://twitter.com/atmega644/status/1082432552403693569

_Thank you!_

VGhlIGNvZGUgaXMgZ3Jvc3MsIG5vb2IteSBhbmQgaW5lZmZpY2llbnQuIEJ1dCBpdCB3b3JrcywgYW5kIGl0J3MgbXkgZmlyc3QgcmVhbCBwcm9qZWN0LiBTbyBJJ20gcHJvdWQgOkQKClRoaXMgaXMgYSBmb3IgbG9vcC4gVGhlIG9ubHkgcGFydCBvZiB0aGlzIGNvZGUgdGhhdCBtYXR0ZXJzIGlzIGF0IHRoZSBib3R0b20uCgpodHRwczovL3R3aXR0ZXIuY29tL0J1c2VzQ2FuRmx5L3N0YXR1cy8xMDgwOTQ5OTkzMTgyMjk0MDE3
