1. /etc/hosts fájlban cserélni kell BME-es címekre

192.168.30.11	bmepaas-master.openshift.local
192.168.30.12	bmepaas-node1.openshift.local
192.168.30.13	bmepaas-node2.openshift.local

2. dnsmasq -ban is be kell állítani a megfelelő IP címeket:

/etc/NetworkManager/dnsmasq.d/wildcard.conf 
address=/localhost.com/127.0.0.1
address=/apps.openshift.local/192.168.30.12
