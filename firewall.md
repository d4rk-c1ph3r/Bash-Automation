# iptables firewall

iptables -L

Append rule to Chain (-A) [INPUT/OUTPUT/FORWARD]
Policy - default rule
(Default policy change)
iptables -P FORWARD DROP   
iptables -A INPUT -s [Source IP/Subnet] -j [DROP/ALLOW] -p [tcp/udp] --destination-port [PORTNUM] 

-D [delete rule from chain]
-I [Adds to the top]

# ufw firewall
sed -i  's/IPV6=yes/IPV6=no/g' /etc/default/ufw
ufw default deny incoming
ufw default allow outgoing
ufw allow ftp
ufw allow ssh
ufw allow http
ufw allow https
ufw allow 8080/tcp
ufw enable
ufw status
