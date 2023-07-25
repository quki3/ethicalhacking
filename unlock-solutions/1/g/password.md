In the final steps, you are going to run a bunch of generated Pairwise Master Keys (PMKs) against the captured packets to get the password. Let me break it down.

A PMK is basically an algorithmic combination of a word and the APs name. Our intention is to continuously generate PMKs using a wordlist against the handshake. If the PMK is valid, the word used to generate it is the password. If the PMK is not valid, it skips to the next word on the list.

I’m going to use the rockyou wordlist located in the /usr/share/wordlists directory. I think this is only found in Kali so if you have a different OS, you might make one of your own manually or generate one using crunch. 

If it isn’t already extracted, just run the command:
`sudo gunzip /usr/share/wordlists/rockyou.txt.gz`

Now run the command:
`sudo aircrack-ng <captured file with .cap> -w <path to wordlist>`

