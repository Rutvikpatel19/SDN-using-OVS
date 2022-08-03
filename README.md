# SDN-using-OVS
We have created a Software define network using OVS controller and a manager.
In this project we have created a SDN using OVS with controller and manager running in a Docker environment.
Following are the requirements for starting this project.
1. Gns3 with vm:
    Download and install GNS3 with the vm on either vmware or virtualbox and runn appliances in VM.
2. Download and install docker linux vm in gns3:
    Go to prefrences > Docker Containers. add a new docker container from docker-hub.com or simply import appliance from the add templet and download the templets from gns store. 
    List of appliance.
     1. Cisco C7200 router
     2. Docker Ubuntu VM
     3. OVS with management interface (Docker with linux interface)
     4. Firefox Browser (to open and interface GUI of Controller and Manager)
     5. Hub to connect everting to NAT cloud
     6. Nat cloud for dynamic ip 
