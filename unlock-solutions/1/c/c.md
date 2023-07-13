### detector, packet sniffer, WEP and WPA/WPA2-PSK cracker and analysis tool for 802.11 wireless LANs
1. 1th option
	- a/ <a href="https://www.aircrack-ng.org/">Aircrack-ng</a>
	- b/ Determine the chipset in your wireless card
		- 	`lspci -vv` or bluethoo `lsusb -vv`
	- c/ Determine the <a href="https://wireless.wiki.kernel.org/en/users/drivers">driver</a>for a wireless card.
		-	`lsusb -vv`- in the last of output see networking controller and check driver in use
		- if you dont have driver you need <a href="https://www.aircrack-ng.org/doku.php?id=install_drivers">install</a> one 
	- <a href="https://www.aircrack-ng.org/doku.php?id=install_aircrack">install</a> Aircrack-ng.
	- `sudo apt install aircrack-ng`
