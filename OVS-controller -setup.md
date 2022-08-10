### Setting controller to eth0 interface.

#### we have use the Management version of the OVS available in Gns3 so that we can control the OVS using a single Interface.

#### Just like the Docker we have to give a static or dynamic IP address to this appliance.

-------

#### Show command to check ovs interface

```bash

ovs-vsctl show #check the port status

ifconfig #check the ip address

```

#### Modify Openflow Protocol

```bash

ovs-vsctl set bridge br0 protocol=OpenFlow13

ovs-vsctl set bridge br0 protocol=OpenFlow10,OpenFlow13

```

#### Connection between Bridge and Controller

#### After TCP type your IP Address.

```bash

ovs-vsctl set-controller br0 tcp:10.10.53.50:6633

```

#### check the controller status

```bash

ovs-vsctl list controller

```

#### If the connection is made to Controller is_connected value will change to true.
