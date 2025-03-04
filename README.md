# OpenWrtAwkScripts
Awk scripts for generating an ethers file from dhcp configuration and for parsing dns debug output.

gen_ethers takes a path to an OpenWrt dhcp configuration file, and generates an ethers file from
  containing MAC addresses and their corresponding device names. This generated output can be put
  in an 'ethers' file in the /etc/ directory of an access point on the network.

dns_data and dns_data_sort take a logfile created by dnsmasq on OpenWrt. They will organize and
  count the dns lookups by device on the network. The sort version sorts the output both by
  device name and by domain name in the device list. The sort version requires gawk to be installed.

