In order to do that you need to first change your wireless card(network interface) from ‘managed’ mode to ‘monitor’ mode. This will turn it from a mere network card to a wireless network reader.First you need to find out the name of your wireless card. Plug in your adapter and run the iwconfig command to find out. It’s usually the last one on the list.
1. - `iwconfig`
- <a href="https://www.aircrack-ng.org/doku.php?id=airmon-ng">airmon-ng</a> is a script that instantly changes your card to monitor mode. You actually can do this manually or make a script of your own but I personally prefer something rather simple.
2. - `sudo airmon-ng check` $check rfkill$ stops processes that could hinder the card from going into monitor mode
3. - `airmon-ng check kill`
4. - `airmon-ng start <network interface>` $start$ tells airmon-ng which network card to execute on
5. - great now you had created a monitor mode called wlan0mon !!!
