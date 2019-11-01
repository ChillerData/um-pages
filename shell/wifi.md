# wifi --
{:data-section="shell"}
{:data-date="November 01, 2019"}
{:data-extra="Um Pages"}

## WPA SUPPLICANT
ip a
: get network interfaces

sudo iwlist wlo1 scan | grep -i ssid
: scan for ssids

sudo wpa\_passphrase networkname password > /etc/wpa\_supplicant/wpa\_supplicant.conf
: add network

sudo systemctl restart wpa\_supplicant
: connect to wifi defined in config

## NMCLI

nmcli c
: list uuids

nmcli dev wifi connect \<ssid\> password \<pass\>
: foo

nmcli c up uuid \<uuid\>
: known connection via uuid

nmcli c up id \<ssid\>
: known connection via ssid

