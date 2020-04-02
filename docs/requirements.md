## Requirements before Helix Sandbox NG installation

Use any local hypervisor like Virtual Box, VMware and KVM or if you need a global Internet access we suggest any Cloud Service Provicer (CSP) like AWS, Azure or Google. 

Minimum server configuration: 1 vCPU, 1GB RAM and 16GB HDD or SSD.

Install any Linux distribution, but Ubuntu Server 18.04.4 LTS has been validated exhaustively for us.

You need to open all the ports below in the firewall settings at your CSP:

```
Port         Transport             Protocol 

22              TCP            SSH 
5000            TCP            Helix Web Interface
1026            TCP            CEF Context Broker 
27000           TCP            MongoDB 
1883            TCP            Eclipse-Mosquitto
4041            TCP            IoT Agent MQTT 
```

### Automated installation (Let us help you with that!)

```
ssh <user>@<helixsandbox IP>
git clone https://github.com/Helix-Platform/Sandbox-NG.git
cd Sandbox-NG
./install.sh
```