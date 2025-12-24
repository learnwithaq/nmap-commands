# nmap-commands
nmap-commands


netdiscover -i eth0 -r 192.168.56.0/24 <br>


nmap -sn 192.168.56.0/24 (Host Discovery)<br>
nmap -p 80 192.168.56.4 (Port scanning on Port 80)<br>
nmap -p 80,443,21 192.168.56.4 (Port Scanning on multiple ports)<br>
nmap -p- 192.168.56.4 (Port Scanning - Scan all ports)<br>
nmap -sV 192.168.56.4 (Scanning Service Version)<br>
nmap -O 192.168.56.4 (Scanning OS Detection)<br>
nmap -A 192.168.56.4 (Scanning - Aggressive Scan (Service Versions, OS Detection, Script Scanning and traceroute<br>
nmap -sV -O -A -T4 192.168.56.4 (Scanning with combined flags)<br>
nmap -sV -O -A -T4 192.168.56.4 -oN results.txt<br>
nmap -sV -O -A -T4 192.168.56.4 -oX results.xml<br>
nmap -Pn -D 192.168.56.115,192.168.56.200,ME,192.168.56.250 192.168.56.108 (Scanning with Decoy IPs)<br>

----------------------------------------------------------------------------------<br>
nmap -sV --script=http-enum.nse google.com -v<br>
nmap -D RND:10 <target ip><br>
nmap -f <target ip><br>
nmap -mtu 24 <target ip><br>
<br>
scanme.nmap.org
