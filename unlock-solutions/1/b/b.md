# what is Packet?
```
/---1byte---/-----21bytes------/---------96bytes----------/
length:		Header			Payload
[header+	|
payload]	|
		|_[ IEEE
		    header][seq.number][destination PAN][destination address][source address]
		  |2 bytes||--1byte---||---2bytes------||-----8bytes--------||----8bytes----|
```
this think above is a basic packet, is the basic unit/building block of data in a computer network.
when data is tranferred from one computer to another, it is broken down and sent in packets.
