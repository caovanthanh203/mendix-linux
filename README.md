# mendix-linux
I am using Ubuntu 20.1
This is tutorial for Mendix developer that use Ubuntu or Linux-base OS (Fedora, openSUSE, Debian,...) 
This contain links to get resources and step to setup.

## What are resources you need?
1. Oracle Virtual Box for Linux
2. Window 10 Image for Virtual Box
3. Mendix Studio Pro installer

## What is requirement?
20 GB minimum diskspace

## Where do you get resources?
1. Oracle Virtual Box for Linux
Link to download: 
https://www.virtualbox.org/wiki/Linux_Downloads
Or with yum:
````
yum install VirtualBox-6.1
````
Or with apt:
````
sudo apt-get update
sudo apt-get install virtualbox-6.1
````
2. Window 10 Image for Virtual Box
Link to download:
https://developer.microsoft.com/en-us/microsoft-edge/tools/vms/

Direct link (may be outdate):
https://az792536.vo.msecnd.net/vms/VMBuild_20190311/VMware/MSEdge/MSEdge.Win10.VMware.zip

3. Mendix Studio Pro:
Link to download: https://marketplace.mendix.com/link/studiopro/

## How to setup?
1. Extract file MSEdge.Win10.VMware.zip, you will see (.ova) file
2. Launch Oracle Virtual Box, import this (.ova) file
![](https://i.ibb.co/6m6My7c/download-38.jpg)
3. Change VM network setting from NAT to Bridge
![](https://i.ibb.co/x6VZdhy/Screenshot-2021-11-15-T144053-913.jpg)
4. Install the Mendix Studio Pro inside VM
To copy you Mendix Studio Pro installer you can copy-paste
Or serve file from your PC via HTTP, and download it on VM using Microsoft Edge in VM
Access PC from VM is [local_network_ip]:port on browser

To serve file, you can use node serve: https://www.npmjs.com/package/serve
````
serve [directory_contain_installer]
````

6. After install you can login, sync, and start Mendix Studio Pro in you VM as a standalone computer
The IP will same your PC IP in local network
![](https://i.ibb.co/9WYFsX5/Screenshot-2021-11-15-T144515-355.jpg)
