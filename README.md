# Set up Technicolor-TG587n in Bridge Mode and Port Mirror

##  Superuser log in credentials for MEO routers:

roosapo

lb5%d$mK

##  Bridge Mode

dns client flush

dns server flush

ppp relay flush

ppp flush

eth flush	

atm flush	

atm  phonebook flush

dhcp server config state disabled

dhcp serverv6 config state disabled

service system list

service system modify name=DNS-C state=disabled

service system modify name=DNS-S state=disabled

firewall config state disabled

saveall

##  Port Mirror

eth switch mirror capture port=2


eth switch mirror ingress port=3 state=enabled

eth switch mirror egress port=3 state=enabled


eth switch mirror ingress port=3 state=disabled

eth switch mirror egress port=3 state=disabled

##  References
https://lehollandaisvolant.net/tout/_misc/telnet/

http://web.archive.org/web/20160326063534/http://npr.me.uk/nbridge.html

http://web.archive.org/web/20160718141727/http://npr.me.uk/forwardports.html

https://forum.meo.pt/internet-fixa-e-movel-11/technicolor-tg582n-v10-2-4-3-telnet-43901#post94882

https://support.aa.net.uk/Category:Router_TG582N
