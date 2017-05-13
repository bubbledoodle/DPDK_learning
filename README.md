# Memory Reservior
The Memory Reservoir system incorporates a local SDN controller and auxiliary external buffer to mitigate the stress on shallow-buffered switches caused by transient traffic fluctuations. To test the system performance, a single rack server based testbed powered by DPDK is built trying to mimic traffic generating and packet scheduling. Current working stages are framework contructions and testbed enviornment establishment. Further more, we would like to acquire system through put statisics implementing different queuing methods or arguments. A more in-detailed mathmatic model needed to be provided on end-to-end delays, propogation delays, some detailed system requirement and so on. 

The project contains two parts of software utilizing, mainly first [DPDK powered applications](http://dpdk.org) and second controller by [moongen](https://github.com/emmericp/MoonGen). The hardware requriement should be 2 wired 10GB/s ports on DPDK campatible NIC. 

## DPDK-essentials
Most parts of documents of DPDK are provided [here](http://dpdk.readthedocs.io/en/v16.04/prog_guide/intro.html), as well as stand alone pktgen application [here](http://pktgen.readthedocs.io/en/latest/getting_started.html). Notice the document may not be the most up-to-date one, so be prepared to modify some parts of the scripts or commands. 

Basic steps of using DPDK:
1. enable hugepage (2MB/1GB)
2. load driver to the kernel (difference)
3. bind NIC to DPDK (script)
4. build application (developer)
5. feed the application with EAL and command, run the application.


