## Before we start the installation we have to give static or dynamic ip to linux docker vm
-----

#### To check internet conectivity.

```bash
ping google.com 
```

#### this will update the repositories and prepare linux for installation.

```bash
apt-get update  
```
#### For this project we will need java version 8 any other version will not work.

```bash
apt-get install openjdk-8-jdk 
```
#### To check Java version

```bash
java -version  #### to check Java version
``` 
#### this open will show you all the given java options available

```bash
update-java-alternatives --list  
```
#### Java export may not work for you plz look for alternatives on internet.

#### this option will add java to you default acces path

```bash 
export JAVA_HOME=$(readlink -f /usr/bin/java | sed "s:bin/java::") 
``` 
 
#### Verification of java installaion

```bash 
echo $JAVA_HOME
```    
  
#### To install all the minimal software files as this verson of docker that we are using will not have all the options in it. 

```bash 
apt install common-software-properties
```   

### This command will download ODL (Open Daylight Controller) which we will you to control OVS
```bash 
wget https://nexus.opendaylight.org/content/groups/public/org/opendaylight/integration/distribution-karaf/0.3.0-Lithium/distribution-karaf-0.3.0-Lithium.tar.gz
```
##### wget command is needed to be installed so use apt-get install wget to install this repository.

#### To unzip file

```bash 
apt install tar
```

```bash 
apt install uzip
```

#navigate to the download folder and look for file name ="distribution-karaf-0.3.0-Lithium.tar.gz" using cd and ls command

#### To unzip the comressed file

```bash 
tar zxvf distribution-karaf-0.3.0-Lithium.tar.gz
``` 

#### After the unzip operation finishes navigate to "distribution-karaf-0.3.0-Lithium" folder

#### This command will download ODL (Open Daylight Controller) which we will you to control OVS

```bash
./bin/karaf # to run open-day-light application
```

#Now at this point you are hosting a apache server on the vm's ip add which is staticaly or dynamicaly assigned.

```bash
feature:install odl-restconf-all odl-openflowplugin-all odl-l2switch-all odl-mdsal-all odl-yangtools-common
```

#### Above command will install necessary features for interfacing the GUI interface of ODL controller

#### To access the GUI connect the controller to a web browers (any web browser running on linux or windows)

#### use following link to acces the web hosted page. "vmsipaddress:8181/index.html" (ip is the eth0 interface ip of the vm)
