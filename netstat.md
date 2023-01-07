# netstat是什么？

netstat（Network Statistics）是在内核中访问网络连接状态及其相关信息的命令行程序，可以显示路由表、实际的网络连接和网络接口设备的状态信息，以及与 IP、TCP、UDP 和 ICMP 协议相关的统计数据，一般用于检验本机各端口的网络服务运行状况。

# 实作一

# Copyright (c) 1993-2004 Microsoft Corp.
#
# This file contains port numbers for well-known services defined by IANA
#
# Format:
#
# <service name>  <port number>/<protocol>  [aliases...]   [#<comment>]
#

echo                7/tcp
echo                7/udp
discard             9/tcp    sink null
discard             9/udp    sink null
systat             11/tcp    users                  #Active users
systat             11/udp    users                  #Active users
daytime            13/tcp
daytime            13/udp
qotd               17/tcp    quote                  #Quote of the day
qotd               17/udp    quote                  #Quote of the day
chargen            19/tcp    ttytst source          #Character generator
chargen            19/udp    ttytst source          #Character generator
ftp-data           20/tcp                           #FTP, data
ftp                21/tcp                           #FTP. control
ssh                22/tcp                           #SSH Remote Login Protocol
telnet             23/tcp
smtp               25/tcp    mail                   #Simple Mail Transfer Protocol
time               37/tcp    timserver
time               37/udp    timserver
rlp                39/udp    resource               #Resource Location Protocol
nameserver         42/tcp    name                   #Host Name Server
nameserver         42/udp    name                   #Host Name Server
nicname            43/tcp    whois
domain             53/tcp                           #Domain Name Server
domain             53/udp                           #Domain Name Server
bootps             67/udp    dhcps                  #Bootstrap Protocol Server
bootpc             68/udp    dhcpc                  #Bootstrap Protocol Client
tftp               69/udp                           #Trivial File Transfer
gopher             70/tcp
finger             79/tcp
http               80/tcp    www www-http           #World Wide Web
hosts2-ns          81/tcp                           #HOSTS2 Name Server
hosts2-ns          81/udp                           #HOSTS2 Name Server
kerberos           88/tcp    krb5 kerberos-sec      #Kerberos
kerberos           88/udp    krb5 kerberos-sec      #Kerberos
hostname          101/tcp    hostnames              #NIC Host Name Server
iso-tsap          102/tcp                           #ISO-TSAP Class 0
rtelnet           107/tcp                           #Remote Telnet Service
pop2              109/tcp    postoffice             #Post Office Protocol - Version 2
pop3              110/tcp                           #Post Office Protocol - Version 3
sunrpc            111/tcp    rpcbind portmap        #SUN Remote Procedure Call
sunrpc            111/udp    rpcbind portmap        #SUN Remote Procedure Call
auth              113/tcp    ident tap              #Identification Protocol
uucp-path         117/tcp
sqlserv           118/tcp                           #SQL Services
nntp              119/tcp    usenet                 #Network News Transfer Protocol
ntp               123/udp                           #Network Time Protocol
epmap             135/tcp    loc-srv                #DCE endpoint resolution
epmap             135/udp    loc-srv                #DCE endpoint resolution
netbios-ns        137/tcp    nbname                 #NETBIOS Name Service
netbios-ns        137/udp    nbname                 #NETBIOS Name Service
netbios-dgm       138/udp    nbdatagram             #NETBIOS Datagram Service
netbios-ssn       139/tcp    nbsession              #NETBIOS Session Service
imap              143/tcp    imap4                  #Internet Message Access Protocol
sql-net           150/tcp
sqlsrv            156/tcp
pcmail-srv        158/tcp                           #PCMail Server
snmp              161/udp                           #SNMP
snmptrap          162/udp    snmp-trap              #SNMP trap
print-srv         170/tcp                           #Network PostScript
bgp               179/tcp                           #Border Gateway Protocol
irc               194/tcp                           #Internet Relay Chat Protocol        
ipx               213/udp                           #IPX over IP
rtsps             322/tcp
rtsps             322/udp
mftp              349/tcp
mftp              349/udp
ldap              389/tcp                           #Lightweight Directory Access Protocol
https             443/tcp    MCom                   #HTTP over TLS/SSL
https             443/udp    MCom                   #HTTP over TLS/SSL
microsoft-ds      445/tcp
microsoft-ds      445/udp
kpasswd           464/tcp                           # Kerberos (v5)
kpasswd           464/udp                           # Kerberos (v5)
isakmp            500/udp    ike                    #Internet Key Exchange
crs               507/tcp                           #Content Replication System
crs               507/udp                           #Content Replication System
exec              512/tcp                           #Remote Process Execution
biff              512/udp    comsat
login             513/tcp                           #Remote Login
who               513/udp    whod
cmd               514/tcp    shell
syslog            514/udp
printer           515/tcp    spooler
talk              517/udp
ntalk             518/udp
efs               520/tcp                           #Extended File Name Server
router            520/udp    route routed
ulp               522/tcp    
ulp               522/udp    
timed             525/udp    timeserver
tempo             526/tcp    newdate
irc-serv          529/tcp
irc-serv          529/udp
courier           530/tcp    rpc
conference        531/tcp    chat
netnews           532/tcp    readnews
netwall           533/udp                           #For emergency broadcasts
uucp              540/tcp    uucpd
klogin            543/tcp                           #Kerberos login
kshell            544/tcp    krcmd                  #Kerberos remote shell
dhcpv6-client     546/tcp                           #DHCPv6 Client
dhcpv6-client     546/udp                           #DHCPv6 Client
dhcpv6-server     547/tcp                           #DHCPv6 Server
dhcpv6-server     547/udp                           #DHCPv6 Server
afpovertcp        548/tcp                           #AFP over TCP
afpovertcp        548/udp                           #AFP over TCP
new-rwho          550/udp    new-who
rtsp              554/tcp                           #Real Time Stream Control Protocol
rtsp              554/udp                           #Real Time Stream Control Protocol
remotefs          556/tcp    rfs rfs_server
rmonitor          560/udp    rmonitord
monitor           561/udp
nntps             563/tcp    snntp                  #NNTP over TLS/SSL
nntps             563/udp    snntp                  #NNTP over TLS/SSL
whoami            565/tcp
whoami            565/udp
ms-shuttle        568/tcp                           #Microsoft shuttle
ms-shuttle        568/udp                           #Microsoft shuttle
ms-rome           569/tcp                           #Microsoft rome
ms-rome           569/udp                           #Microsoft rome
http-rpc-epmap    593/tcp                           #HTTP RPC Ep Map
http-rpc-epmap    593/udp                           #HTTP RPC Ep Map
hmmp-ind          612/tcp                           #HMMP Indication
hmmp-ind          612/udp                           #HMMP Indication
hmmp-op           613/tcp                           #HMMP Operation
hmmp-op           613/udp                           #HMMP Operation
ldaps             636/tcp    sldap                  #LDAP over TLS/SSL
doom              666/tcp                           #Doom Id Software
doom              666/udp                           #Doom Id Software
msexch-routing    691/tcp                           #MS Exchange Routing
msexch-routing    691/udp                           #MS Exchange Routing
kerberos-adm      749/tcp                           #Kerberos administration
kerberos-adm      749/udp                           #Kerberos administration
kerberos-iv       750/udp                           #Kerberos version IV
mdbs_daemon       800/tcp
mdbs_daemon       800/udp
ftps-data         989/tcp                           #FTP data, over TLS/SSL
ftps              990/tcp                           #FTP control, over TLS/SSL
telnets           992/tcp                           #Telnet protocol over TLS/SSL
imaps             993/tcp                           #IMAP4 protocol over TLS/SSL
ircs              994/tcp                           #IRC protocol over TLS/SSL
pop3s             995/tcp    spop3                  #pop3 protocol over TLS/SSL (was spop3)
pop3s             995/udp    spop3                  #pop3 protocol over TLS/SSL (was spop3)
kpop             1109/tcp                           #Kerberos POP
nfsd-status      1110/tcp                           #Cluster status info
nfsd-keepalive   1110/udp                           #Client status info
nfa              1155/tcp                           #Network File Access
nfa              1155/udp                           #Network File Access
activesync       1034/tcp                           #ActiveSync Notifications
phone            1167/udp                           #Conference calling
opsmgr           1270/tcp                           #Microsoft Operations Manager
opsmgr           1270/udp                           #Microsoft Operations Manager
ms-sql-s         1433/tcp                           #Microsoft-SQL-Server 
ms-sql-s         1433/udp                           #Microsoft-SQL-Server 
ms-sql-m         1434/tcp                           #Microsoft-SQL-Monitor
ms-sql-m         1434/udp                           #Microsoft-SQL-Monitor                
ms-sna-server    1477/tcp
ms-sna-server    1477/udp
ms-sna-base      1478/tcp
ms-sna-base      1478/udp
wins             1512/tcp                           #Microsoft Windows Internet Name Service
wins             1512/udp                           #Microsoft Windows Internet Name Service
ingreslock       1524/tcp    ingres
stt              1607/tcp
stt              1607/udp
l2tp             1701/udp                           #Layer Two Tunneling Protocol
pptconference    1711/tcp
pptconference    1711/udp
pptp             1723/tcp                           #Point-to-point tunnelling protocol
msiccp           1731/tcp
msiccp           1731/udp
remote-winsock   1745/tcp
remote-winsock   1745/udp
ms-streaming     1755/tcp
ms-streaming     1755/udp
msmq             1801/tcp                           #Microsoft Message Queue
msmq             1801/udp                           #Microsoft Message Queue
radius           1812/udp                           #RADIUS authentication protocol
radacct          1813/udp                           #RADIUS accounting protocol
msnp             1863/tcp
msnp             1863/udp
ssdp             1900/tcp
ssdp             1900/udp
close-combat     1944/tcp
close-combat     1944/udp
nfsd             2049/udp    nfs                    #NFS server
knetd            2053/tcp                           #Kerberos de-multiplexor
mzap             2106/tcp                           #Multicast-Scope Zone Announcement Protocol
mzap             2106/udp                           #Multicast-Scope Zone Announcement Protocol
qwave            2177/tcp                           #QWAVE
qwave            2177/udp                           #QWAVE Experiment Port
directplay       2234/tcp                           #DirectPlay
directplay       2234/udp                           #DirectPlay
ms-olap3         2382/tcp                           #Microsoft OLAP 3
ms-olap3         2382/udp                           #Microsoft OLAP 3
ms-olap4         2383/tcp                           #Microsoft OLAP 4
ms-olap4         2383/udp                           #Microsoft OLAP 4
ms-olap1         2393/tcp                           #Microsoft OLAP 1
ms-olap1         2393/udp                           #Microsoft OLAP 1
ms-olap2         2394/tcp                           #Microsoft OLAP 2
ms-olap2         2394/udp                           #Microsoft OLAP 2
ms-theater       2460/tcp
ms-theater       2460/udp
wlbs             2504/tcp                           #Microsoft Windows Load Balancing Server
wlbs             2504/udp                           #Microsoft Windows Load Balancing Server
ms-v-worlds      2525/tcp                           #Microsoft V-Worlds 
ms-v-worlds      2525/udp                           #Microsoft V-Worlds 
sms-rcinfo       2701/tcp                           #SMS RCINFO
sms-rcinfo       2701/udp                           #SMS RCINFO
sms-xfer         2702/tcp                           #SMS XFER
sms-xfer         2702/udp                           #SMS XFER
sms-chat         2703/tcp                           #SMS CHAT
sms-chat         2703/udp                           #SMS CHAT
sms-remctrl      2704/tcp                           #SMS REMCTRL
sms-remctrl      2704/udp                           #SMS REMCTRL
msolap-ptp2      2725/tcp                           #MSOLAP PTP2
msolap-ptp2      2725/udp                           #MSOLAP PTP2
icslap           2869/tcp
icslap           2869/udp
cifs             3020/tcp
cifs             3020/udp
xbox             3074/tcp                           #Microsoft Xbox game port
xbox             3074/udp                           #Microsoft Xbox game port
ms-dotnetster    3126/tcp                           #Microsoft .NET ster port
ms-dotnetster    3126/udp                           #Microsoft .NET ster port
ms-rule-engine   3132/tcp                           #Microsoft Business Rule Engine Update Service
ms-rule-engine   3132/udp                           #Microsoft Business Rule Engine Update Service
msft-gc          3268/tcp                           #Microsoft Global Catalog
msft-gc          3268/udp                           #Microsoft Global Catalog
msft-gc-ssl      3269/tcp                           #Microsoft Global Catalog with LDAP/SSL
msft-gc-ssl      3269/udp                           #Microsoft Global Catalog with LDAP/SSL
ms-cluster-net   3343/tcp                           #Microsoft Cluster Net
ms-cluster-net   3343/udp                           #Microsoft Cluster Net
ms-wbt-server    3389/tcp                           #MS WBT Server
ms-wbt-server    3389/udp                           #MS WBT Server
ms-la            3535/tcp                           #Microsoft Class Server
ms-la            3535/udp                           #Microsoft Class Server
pnrp-port        3540/tcp                           #PNRP User Port
pnrp-port        3540/udp                           #PNRP User Port
teredo           3544/tcp                           #Teredo Port
teredo           3544/udp                           #Teredo Port
p2pgroup         3587/tcp                           #Peer to Peer Grouping
p2pgroup         3587/udp                           #Peer to Peer Grouping
ws-discovery     3702/udp                           #WS-Discovery
ws-discovery     3702/tcp                           #WS-Discovery
dvcprov-port     3776/tcp                           #Device Provisioning Port
dvcprov-port     3776/udp                           #Device Provisioning Port
msfw-control     3847/tcp                           #Microsoft Firewall Control
msdts1           3882/tcp                           #DTS Service Port
sdp-portmapper   3935/tcp                           #SDP Port Mapper Protocol
sdp-portmapper   3935/udp                           #SDP Port Mapper Protocol
net-device       4350/tcp                           #Net Device
net-device       4350/udp                           #Net Device
ipsec-msft       4500/tcp                           #Microsoft IPsec NAT-T
ipsec-msft       4500/udp                           #Microsoft IPsec NAT-T
llmnr            5355/tcp                           #LLMNR 
llmnr            5355/udp                           #LLMNR 
wsd              5357/tcp                           #Web Services on devices 
wsd              5358/tcp                           #Web Services on devices
rrac             5678/tcp                           #Remote Replication Agent Connection
rrac             5678/udp                           #Remote Replication Agent Connection
dccm             5679/tcp                           #Direct Cable Connect Manager
dccm             5679/udp                           #Direct Cable Connect Manager
ms-licensing     5720/tcp                           #Microsoft Licensing
ms-licensing     5720/udp                           #Microsoft Licensing 
directplay8      6073/tcp                           #DirectPlay8
directplay8      6073/udp                           #DirectPlay8
ms-do            7680/tcp                           #Microsoft Delivery Optimization
ms-do            7680/udp                           #Microsoft Delivery Optimization
man              9535/tcp                           #Remote Man Server
rasadv           9753/tcp
rasadv           9753/udp
imip-channels   11320/tcp                           #IMIP Channels Port
imip-channels   11320/udp                           #IMIP Channels Port
directplaysrvr  47624/tcp                           #Direct Play Server
directplaysrvr  47624/udp                           #Direct Play Server



常用服务：9753/tcp  47624/udp

不同的服务可以用相同的接口，同一服务的接口服务不是唯一的。

# 实作二

Microsoft Windows [版本 10.0.22000.1219]
(c) Microsoft Corporation。保留所有权利。

C:\Users\Mr.hu>netstat -an

活动连接

  协议  本地地址          外部地址        状态
  TCP    0.0.0.0:135            0.0.0.0:0              LISTENING
  TCP    0.0.0.0:445            0.0.0.0:0              LISTENING
  TCP    0.0.0.0:902            0.0.0.0:0              LISTENING
  TCP    0.0.0.0:912            0.0.0.0:0              LISTENING
  TCP    0.0.0.0:3306           0.0.0.0:0              LISTENING
  TCP    0.0.0.0:5040           0.0.0.0:0              LISTENING
  TCP    0.0.0.0:27036          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:30531          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:49664          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:49665          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:49666          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:49667          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:49668          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:49700          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:61771          0.0.0.0:0              LISTENING
  TCP    127.0.0.1:4301         0.0.0.0:0              LISTENING
  TCP    127.0.0.1:4709         0.0.0.0:0              LISTENING
  TCP    127.0.0.1:8680         0.0.0.0:0              LISTENING
  TCP    127.0.0.1:10000        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:10067        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:11066        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:13010        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:13030        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:13031        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:13032        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:16308        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:16308        127.0.0.1:49787        ESTABLISHED
  TCP    127.0.0.1:17532        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:17532        127.0.0.1:49695        ESTABLISHED
  TCP    127.0.0.1:17945        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:22112        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:27060        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:49669        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:49695        127.0.0.1:17532        ESTABLISHED
  TCP    127.0.0.1:49787        127.0.0.1:16308        ESTABLISHED
  TCP    127.0.0.1:50815        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:51281        127.0.0.1:54533        ESTABLISHED
  TCP    127.0.0.1:51282        127.0.0.1:51283        ESTABLISHED
  TCP    127.0.0.1:51283        127.0.0.1:51282        ESTABLISHED
  TCP    127.0.0.1:54530        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:54533        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:54533        127.0.0.1:51281        ESTABLISHED
  TCP    192.168.0.104:139      0.0.0.0:0              LISTENING
  TCP    192.168.0.104:49160    183.47.107.151:443     CLOSE_WAIT
  TCP    192.168.0.104:49711    121.40.155.17:443      ESTABLISHED
  TCP    192.168.0.104:49722    20.198.162.76:443      ESTABLISHED
  TCP    192.168.0.104:49809    47.110.135.163:443     ESTABLISHED
  TCP    192.168.0.104:49892    118.178.225.181:443    CLOSE_WAIT
  TCP    192.168.0.104:50049    119.84.169.100:443     CLOSE_WAIT
  TCP    192.168.0.104:50072    110.43.89.215:80       CLOSE_WAIT
  TCP    192.168.0.104:50584    113.96.202.106:80      ESTABLISHED
  TCP    192.168.0.104:50841    121.36.2.168:443       CLOSE_WAIT
  TCP    192.168.0.104:50842    121.36.106.50:443      CLOSE_WAIT
  TCP    192.168.0.104:50843    121.36.2.168:443       CLOSE_WAIT
  TCP    192.168.0.104:50844    121.36.2.168:443       CLOSE_WAIT
  TCP    192.168.0.104:51146    119.84.171.1:443       CLOSE_WAIT
  TCP    192.168.0.104:51156    34.117.59.81:443       ESTABLISHED
  TCP    192.168.0.104:51390    14.18.180.162:443      CLOSE_WAIT
  TCP    192.168.0.104:51517    58.49.216.78:443       CLOSE_WAIT
  TCP    192.168.0.104:51605    202.89.233.101:443     TIME_WAIT
  TCP    192.168.0.104:51609    20.205.69.80:443       ESTABLISHED
  TCP    192.168.0.104:51621    14.18.180.113:443      CLOSE_WAIT
  TCP    192.168.0.104:51628    165.22.214.237:443     CLOSE_WAIT
  TCP    192.168.0.104:51629    20.189.173.10:443      ESTABLISHED
  TCP    192.168.0.104:51631    125.72.129.221:80      TIME_WAIT
  TCP    192.168.0.104:51645    23.2.128.171:443       ESTABLISHED
  TCP    192.168.0.104:51646    118.123.102.107:443    ESTABLISHED
  TCP    192.168.0.104:51651    23.210.215.97:80       TIME_WAIT
  TCP    192.168.0.104:51663    183.2.143.108:443      ESTABLISHED
  TCP    192.168.0.104:51665    14.215.177.38:80       FIN_WAIT_1
  TCP    192.168.0.104:51668    14.215.177.38:80       FIN_WAIT_1
  TCP    192.168.0.104:57862    113.240.72.111:443     CLOSE_WAIT
  TCP    192.168.0.104:58815    103.28.54.181:27025    ESTABLISHED
  TCP    192.168.0.104:61469    183.3.235.214:443      CLOSE_WAIT
  TCP    192.168.0.104:61607    183.66.105.139:443     CLOSE_WAIT
  TCP    192.168.0.104:61765    119.3.178.178:21111    ESTABLISHED
  TCP    192.168.0.104:62376    113.96.237.69:443      CLOSE_WAIT
  TCP    192.168.0.104:62532    183.47.104.208:8080    ESTABLISHED
  TCP    192.168.0.104:62559    14.18.180.113:443      CLOSE_WAIT
  TCP    192.168.0.104:62568    183.47.103.244:443     CLOSE_WAIT
  TCP    192.168.0.104:62570    183.47.126.96:443      CLOSE_WAIT
  TCP    192.168.0.104:62572    183.47.103.136:443     CLOSE_WAIT
  TCP    192.168.0.104:62573    183.47.103.134:443     CLOSE_WAIT
  TCP    192.168.0.104:62575    183.47.107.190:443     CLOSE_WAIT
  TCP    192.168.0.104:62576    183.47.103.247:443     CLOSE_WAIT
  TCP    192.168.0.104:62577    183.47.109.208:443     CLOSE_WAIT
  TCP    192.168.0.104:62578    183.47.107.228:443     CLOSE_WAIT
  TCP    192.168.0.104:62583    119.147.190.77:443     CLOSE_WAIT
  TCP    192.168.0.104:62584    183.60.230.59:443      CLOSE_WAIT
  TCP    192.168.0.104:62589    123.151.54.57:8080     ESTABLISHED
  TCP    192.168.0.104:62614    117.62.242.202:443     ESTABLISHED
  TCP    192.168.0.104:62618    183.47.102.180:14000   ESTABLISHED
  TCP    192.168.0.104:62619    183.47.98.92:8080      ESTABLISHED
  TCP    192.168.0.104:62630    42.81.184.252:80       ESTABLISHED
  TCP    192.168.0.104:62633    183.66.105.12:443      ESTABLISHED
  TCP    192.168.0.104:62666    14.18.180.113:443      CLOSE_WAIT
  TCP    192.168.0.104:62667    14.18.180.113:443      CLOSE_WAIT
  TCP    192.168.0.104:62668    14.18.180.113:443      CLOSE_WAIT
  TCP    192.168.0.104:62853    118.121.192.67:443     CLOSE_WAIT
  TCP    192.168.0.104:63034    14.18.180.247:443      CLOSE_WAIT
  TCP    192.168.0.104:64296    183.47.104.186:443     CLOSE_WAIT
  TCP    192.168.0.104:65178    119.84.171.1:443       CLOSE_WAIT
  TCP    192.168.0.104:65484    110.43.120.11:443      CLOSE_WAIT
  TCP    192.168.50.1:139       0.0.0.0:0              LISTENING
  TCP    192.168.86.1:139       0.0.0.0:0              LISTENING
  TCP    [::]:135               [::]:0                 LISTENING
  TCP    [::]:445               [::]:0                 LISTENING
  TCP    [::]:3306              [::]:0                 LISTENING
  TCP    [::]:49664             [::]:0                 LISTENING
  TCP    [::]:49665             [::]:0                 LISTENING
  TCP    [::]:49666             [::]:0                 LISTENING
  TCP    [::]:49667             [::]:0                 LISTENING
  TCP    [::]:49668             [::]:0                 LISTENING
  TCP    [::]:49700             [::]:0                 LISTENING
  TCP    [::]:61771             [::]:0                 LISTENING
  UDP    0.0.0.0:123            *:*
  UDP    0.0.0.0:500            *:*
  UDP    0.0.0.0:4008           *:*
  UDP    0.0.0.0:4500           *:*
  UDP    0.0.0.0:5050           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5355           *:*
  UDP    0.0.0.0:15869          *:*
  UDP    0.0.0.0:27036          *:*
  UDP    0.0.0.0:50020          *:*
  UDP    0.0.0.0:50225          *:*
  UDP    0.0.0.0:50233          *:*
  UDP    0.0.0.0:50724          *:*
  UDP    0.0.0.0:51473          *:*
  UDP    0.0.0.0:51660          *:*
  UDP    0.0.0.0:51964          *:*
  UDP    0.0.0.0:52224          *:*
  UDP    0.0.0.0:53222          172.67.143.53:443
  UDP    0.0.0.0:54920          *:*
  UDP    0.0.0.0:56017          *:*
  UDP    0.0.0.0:57044          *:*
  UDP    0.0.0.0:59852          *:*
  UDP    0.0.0.0:61186          *:*
  UDP    0.0.0.0:63640          *:*
  UDP    127.0.0.1:1900         *:*
  UDP    127.0.0.1:40000        *:*
  UDP    127.0.0.1:50060        *:*
  UDP    127.0.0.1:50219        *:*
  UDP    127.0.0.1:50220        *:*
  UDP    127.0.0.1:50221        *:*
  UDP    127.0.0.1:50222        *:*
  UDP    127.0.0.1:50223        *:*
  UDP    127.0.0.1:50224        *:*
  UDP    127.0.0.1:51179        127.0.0.1:51180
  UDP    127.0.0.1:51180        127.0.0.1:51179
  UDP    127.0.0.1:51573        127.0.0.1:51574
  UDP    127.0.0.1:51574        127.0.0.1:51573
  UDP    127.0.0.1:54680        127.0.0.1:54681
  UDP    127.0.0.1:54681        127.0.0.1:54680
  UDP    127.0.0.1:54682        127.0.0.1:54683
  UDP    127.0.0.1:54683        127.0.0.1:54682
  UDP    127.0.0.1:54684        127.0.0.1:54685
  UDP    127.0.0.1:54685        127.0.0.1:54684
  UDP    127.0.0.1:54922        127.0.0.1:54923
  UDP    127.0.0.1:54923        127.0.0.1:54922
  UDP    127.0.0.1:54924        127.0.0.1:54925
  UDP    127.0.0.1:54925        127.0.0.1:54924
  UDP    127.0.0.1:54926        127.0.0.1:54927
  UDP    127.0.0.1:54927        127.0.0.1:54926
  UDP    127.0.0.1:54928        127.0.0.1:54929
  UDP    127.0.0.1:54929        127.0.0.1:54928
  UDP    127.0.0.1:54930        127.0.0.1:54931
  UDP    127.0.0.1:54931        127.0.0.1:54930
  UDP    127.0.0.1:54932        127.0.0.1:54933
  UDP    127.0.0.1:54933        127.0.0.1:54932
  UDP    127.0.0.1:54937        127.0.0.1:54938
  UDP    127.0.0.1:54938        127.0.0.1:54937
  UDP    127.0.0.1:56022        127.0.0.1:56023
  UDP    127.0.0.1:56023        127.0.0.1:56022
  UDP    127.0.0.1:56024        127.0.0.1:56025
  UDP    127.0.0.1:56025        127.0.0.1:56024
  UDP    127.0.0.1:56026        127.0.0.1:56027
  UDP    127.0.0.1:56027        127.0.0.1:56026
  UDP    127.0.0.1:56290        *:*
  UDP    127.0.0.1:56291        *:*
  UDP    127.0.0.1:56292        *:*
  UDP    127.0.0.1:56293        *:*
  UDP    127.0.0.1:58025        127.0.0.1:58026
  UDP    127.0.0.1:58026        127.0.0.1:58025
  UDP    127.0.0.1:60617        127.0.0.1:60618
  UDP    127.0.0.1:60618        127.0.0.1:60617
  UDP    127.0.0.1:60961        *:*
  UDP    127.0.0.1:60962        *:*
  UDP    127.0.0.1:60963        *:*
  UDP    127.0.0.1:60964        *:*
  UDP    127.0.0.1:60973        *:*
  UDP    127.0.0.1:60974        *:*
  UDP    127.0.0.1:60975        *:*
  UDP    127.0.0.1:60976        *:*
  UDP    127.0.0.1:61003        *:*
  UDP    127.0.0.1:61004        *:*
  UDP    127.0.0.1:61005        *:*
  UDP    127.0.0.1:61006        *:*
  UDP    127.0.0.1:61190        127.0.0.1:61191
  UDP    127.0.0.1:61191        127.0.0.1:61190
  UDP    127.0.0.1:61193        127.0.0.1:61194
  UDP    127.0.0.1:61194        127.0.0.1:61193
  UDP    127.0.0.1:61195        127.0.0.1:61196
  UDP    127.0.0.1:61196        127.0.0.1:61195
  UDP    169.254.223.200:54936  *:*
  UDP    192.168.0.104:137      *:*
  UDP    192.168.0.104:138      *:*
  UDP    192.168.0.104:1900     *:*
  UDP    192.168.0.104:5657     *:*
  UDP    192.168.0.104:50057    *:*
  UDP    192.168.0.104:54679    *:*
  UDP    192.168.0.104:56021    *:*
  UDP    192.168.50.1:137       *:*
  UDP    192.168.50.1:138       *:*
  UDP    192.168.50.1:1900      *:*
  UDP    192.168.50.1:50058     *:*
  UDP    192.168.86.1:137       *:*
  UDP    192.168.86.1:138       *:*
  UDP    192.168.86.1:1900      *:*
  UDP    192.168.86.1:50059     *:*
  UDP    [::]:123               *:*
  UDP    [::]:500               *:*
  UDP    [::]:4500              *:*
  UDP    [::]:5353              *:*
  UDP    [::]:5353              *:*
  UDP    [::]:5353              *:*
  UDP    [::]:5353              *:*
  UDP    [::]:5355              *:*
  UDP    [::]:50225             *:*
  UDP    [::]:50233             *:*
  UDP    [::]:50724             *:*
  UDP    [::]:51473             *:*
  UDP    [::]:51660             *:*
  UDP    [::]:51964             *:*
  UDP    [::]:57044             *:*
  UDP    [::]:59852             *:*
  UDP    [::]:61186             *:*
  UDP    [::]:63640             *:*
  UDP    [::1]:1900             *:*
  UDP    [::1]:50056            *:*
  UDP    [fe80::293d:8e2f:8559:5c2%4]:1900  *:*
  UDP    [fe80::293d:8e2f:8559:5c2%4]:50053  *:*
  UDP    [fe80::36c3:a98b:955b:884f%19]:1900  *:*
  UDP    [fe80::36c3:a98b:955b:884f%19]:50054  *:*
  UDP    [fe80::fb65:9fd2:30c3:b25c%11]:1900  *:*
  UDP    [fe80::fb65:9fd2:30c3:b25c%11]:50055  *:*

C:\Users\Mr.hu>
