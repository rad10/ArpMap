# ArpMap
Network mapping system that uses arp packets

**!! requires arp-scan and nmap to run !!**

This program uses the two programs ``NMap`` and ``Arp-Scan`` to quickly find machines on a network and identify them. Arp-scan is used to get the currently active machines on the network and NMap is used to get their name as well as confirm their active existance.

This program is made to work for linux and linux alone (Currently).

### Help and Options

> ArpMap [OPTION] [IPADDRESS]

>> ArpMap is a program made to scan a list of ip's and return a list of alive hosts and their names. This program is dependant on nmap and its functions to properly work.

>> Options:

>>> -f | (-)-file			Input ip list from file.

>>> -tl | (-)-textlist [default]	Input ip's. It can be 1 or more, but to have you multiple it must be in quotes and there has to be a space in between each ip address. You can also scan multiple addresses with a - in between the numbers.
Example: ``123.456.789.101 987.654.321.012`` ``123.832.1.0-255 101.204.294.103``

>>> -ln | (-)-local			Scans entire local network. No given ip address is required.

>>> -vi | (-)-visual [default]	Gives you a visual with alive machine ip's and names. It is on by default

>>> -t				simple output. Doesn't give names, but gives alive ips in list to be used by other program.

>>> -r				Adds -Pn command to NMap script.

>>> -i*				interface to read from to find ip addresses.
