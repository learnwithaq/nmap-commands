# nmap-commands
nmap-commands


netdiscover -i eth0 -r 192.168.56.0/24


nmap -sn 192.168.56.0/24 (Host Discovery)
nmap -p 80 192.168.56.4 (Port scanning on Port 80)
nmap -p 80,443,21 192.168.56.4 (Port Scanning on multiple ports)
nmap -p- 192.168.56.4 (Port Scanning - Scan all ports)
nmap -sV 192.168.56.4 (Scanning Service Version)
nmap -O 192.168.56.4 (Scanning OS Detection)
nmap -A 192.168.56.4 (Scanning - Aggressive Scan (Service Versions, OS Detection, Script Scanning and traceroute
nmap -sV -O -A -T4 192.168.56.4 (Scanning with combined flags)
nmap -sV -O -A -T4 192.168.56.4 -oN results.txt
nmap -sV -O -A -T4 192.168.56.4 -oX results.xml
nmap -Pn -D 192.168.56.115,192.168.56.200,ME,192.168.56.250 192.168.56.108 (Scanning with Decoy IPs)

----------------------------------------------------------------------------------
nmap -sV --script=http-enum.nse google.com -v
nmap -D RND:10 <target ip>
nmap -f <target ip>
nmap -mtu 24 <target ip>

scanme.nmap.org
