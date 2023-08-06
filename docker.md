### docker

#### container
<img width="622" alt="image" src="https://github.com/Dhanush-krish/docker-kubernetes/assets/58057080/ea1f3d1a-939b-4807-b9ee-ed9bc97c5ad7">

A **hypervisor** is software that creates and runs virtual machines (VMs), allows one host computer to support multiple guest VMs by virtually sharing its resources, such as memory and processing.


* lightweight VM
* process running in a isolated environment
* Namespaces
  * mnt/file system
  * network
  * uts
  * pid
  * ipc
  * user
* CGroups - Controlled Groups
    * controls and monitors like CPU, Memory, Disk, Network
* layers - Union File System[UFS]  - OverlayFS2
* Image are mounted read-only and each cointainer has its own changes. 
