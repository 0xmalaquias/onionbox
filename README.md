# [ onionbox ]
[*] Deep Bash based proxy automation for linux distros, (uses Tor and firewall rules).

[*] Supports open-rc, systemd, runit for service managment on boot.

[*] Firewall rules are iptables based, translated to nftables by useing iptables-nft module, disables icmp-echo-request (pings) and allowing traffic/communication only trough tor.

[!] Required PKGs: 
- openbsd-netcat curl tor iptables iproute2 networkmanager e2fsprogs coreutils util-linux bash iptables-nft nftables sudo nyx

[!] Script actions: --start, --stop, --restart, --status, --boot-enable, --boot-disable, --myip, --change, --fix, --set-bridges --restart-torrc, --help.

[!] To use it right now: 
- Note: always run this as root, (if you have sudo/git installed on your system)
- git clone https://github.com/NewMaster27/onionbox && cd onionbox && chmod +x * && ./onionbox help

[!] In addition:
- Recommended: Configure a secure non standard/common browser(like tor's one, it is easy). 
- Recommended: Use Tor bridges or a VPN connection, just in case you want to be 100% sure that your ISP wont be able to see your connection nodes!!
