###  Before we start the installation we have to give static or dynamic ip to linux docker vm

#### Update the Repositories 
```bash
apt-get update
```

#### Installing some basic software properties

``` bash
apt-get install -y bash-completion software-properties-common python-software-properties
```
#### Install Curl
```bash
apt install curl
```
#### script to install Node JS 4.x
```bash
curl -sl https://deb.nodesource.com/setup_4.x | sudo -E bash -
```

#### install Node JS
```bash
apt-get install nodejs
```
#### Git clone download
```bash
git clone https://github.com/CiscoDevNet/OpenDaylight-Openflow-App.git
```
#### Set controller IP address in Manager
```bash
sed -i 's/localhost/<server_ip>/g' ./OpenDaylight-Openflow-App/ofm/src/common/config/env.module.js ### Use the IP we noted earlier, for "server_ip"
```

#### Install NPM and other software's
```bash
apt install npm
npm install -g grunt-cli
``` 

#### change directory to the OFM File
```bash
cd OpenDaylight-Openflow-App
```
#### Activate Apache server
```bash
grunt
```
### "http://localhost:9000" will display.
#### here the local host is your manager pc's ip 

#### OFM is ready.
