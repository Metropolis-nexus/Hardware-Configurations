## iDRAC Settings

- Do **NOT** disable RedFish - iDRAC needs it to work internally.
- Set iDRAC hostname with racadm through SSH.

### Overview

- User Interface Title Bar Information -> System Host Name

### Connectivity

#### Network

- iDRAC Auto Discovery -> Disable
- Register iDRAC on DNS -> Disable
- DNS iDRAC Name -> idrac
- Static DNS name -> Set approprieate DNS name
- Auto Config -> DHCP Provisioning -> Disabled
- IPv4 Settings -> Disable DHCP, use 1.1.1.2 and 1.0.0.2 as DNS servers
- IPv6 Settings -> Disable Autoconfiguration, use 2606:4700:4700::1111 and 2606:4700:4700::1001 as DNS servers

#### Serial Over LAN
- Disable Serial Over LAN

### Services

#### Web Server
- HTTP/2 Protocol -> Enabled
- Block HTTP Port -> Enabled
- SSL Encryption -> 256-Bit or higher
- TLS Protocol -> TLS 1.3 Only

#### SSH
- Disable SSH

#### Remote RACADM
- Disable Remote RACADM

#### SNMP Agent
- Disable SNMP Agent

#### Automated System Recovery Agent
- Disable Automated System Recovery Agent

### Users

#### Global User Settings
- Set password policy to strong

### Settings

#### Time Zone and NTP Settings
- Timezone -> Set to UTC
- Enable NTP 
- Use time.cloudflare.com

#### Management USB Settings
- Disable iDRAC Managed: USB SCP