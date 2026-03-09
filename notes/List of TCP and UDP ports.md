both [[Transmission Control Protocol (TCP)|TCP]] and [[User Datagram Protocol (UDP)|UDP]] only need one [[Port (computer networking)|port]] for [[Duplex (telecommunications)|bidirectional]] traffic. TCP usually uses port numbers that match the services of the corresponding UDP implementations, if they exist, and vice versa.

the [[Internet Assigned Numbers Authority (IANA)]] is responsible for maintaining the official assignments of port numbers for specific uses; however, many unofficial uses of both well-known and registered port numbers occur in practice.

(see also [[TCP vs UDP]])

# Port ranges

| Range         | Name                |
| ------------- | ------------------- |
| 0 – 1023      | Well-known ports    |
| 1024 – 49151  | Registered ports    |
| 49152 – 65535 | Dynamic / ephemeral |

# Full Well-Known Port Table (common ones)

|Port|Service|Description|
|---|---|---|
|0|Reserved|Reserved|
|1|TCPMUX|TCP Port Service Multiplexer|
|5|RJE|Remote Job Entry|
|7|Echo|Echo service|
|9|Discard|Discards received packets|
|11|SYSTAT|Active users|
|13|Daytime|Returns date/time|
|15|Netstat|Network status|
|17|QOTD|Quote of the Day|
|18|MSP|Message Send Protocol|
|19|Chargen|Character Generator|
|20|FTP Data|File transfer data|
|21|FTP|File Transfer Protocol|
|22|SSH|Secure Shell|
|23|Telnet|Remote terminal login|
|25|SMTP|Email sending|
|37|Time|Time protocol|
|42|WINS|Windows Internet Naming|
|43|WHOIS|Domain lookup|
|49|TACACS|Cisco authentication|
|53|DNS|Domain Name System|
|67|DHCP Server|DHCP service|
|68|DHCP Client|DHCP client|
|69|TFTP|Trivial File Transfer|
|70|Gopher|Early web protocol|
|79|Finger|User information|
|80|HTTP|Web traffic|
|88|Kerberos|Authentication|
|95|SUPDUP|Terminal protocol|
|101|HOSTNAME|Hostname service|
|102|ISO-TSAP|ISO transport|
|107|RTELNET|Remote telnet|
|109|POP2|Post Office Protocol v2|
|110|POP3|Email retrieval|
|111|RPCBind|Remote procedure calls|
|113|Ident|Authentication service|
|119|NNTP|Network news transfer|
|123|NTP|Network Time Protocol|
|135|MS RPC|Microsoft RPC|
|137|NetBIOS Name|Windows name service|
|138|NetBIOS Datagram|Windows datagram|
|139|NetBIOS Session|Windows session|
|143|IMAP|Email synchronization|
|161|SNMP|Network management|
|162|SNMP Trap|SNMP alerts|
|179|BGP|Border Gateway Protocol|
|194|IRC|Internet Relay Chat|
|201|AppleTalk|Apple networking|
|209|QMTP|Quick Mail Transfer|
|213|IPX|Novell networking|
|220|IMAP3|Email protocol|
|389|LDAP|Directory services|
|427|SLP|Service location protocol|
|443|HTTPS|Secure web|
|444|SNPP|Paging protocol|
|445|SMB|Windows file sharing|
|464|Kerberos Password|Kerberos change|
|465|SMTPS|Secure SMTP|
|500|ISAKMP|VPN key exchange|
|512|rexec|Remote execution|
|513|rlogin|Remote login|
|514|Syslog|Logging|
|515|LPD|Printer service|
|520|RIP|Routing Information Protocol|
|521|RIPng|RIP for IPv6|
|540|UUCP|Unix to Unix copy|
|548|AFP|Apple file protocol|
|554|RTSP|Streaming control|
|563|NNTPS|Secure NNTP|
|587|SMTP Submission|Email submission|
|591|FileMaker|Database|
|593|HTTP RPC|Microsoft RPC|
|636|LDAPS|Secure LDAP|
|639|MSDP|Multicast source discovery|
|646|LDP|Label distribution protocol|
|647|DHCP Failover|DHCP failover|
|691|Microsoft Exchange Routing||
|860|iSCSI||
|873|rsync||
|902|VMware Server||
|989|FTPS Data||
|990|FTPS Control||
|993|IMAPS||
|995|POP3S||
