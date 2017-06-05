# mesosphere-universe-oneview

Coming soon -- Please check back in a few days.

This github repository contains HPE Image Streamer artifacts as well as Mesosphere Enterprise DC/OS service definitions to enable an integration between DC/OS and HPE Synergy.

The HPE OneView Universe app when installed from the DC/OS Universe will provides the following services

- Verify that the HPE OneView service is live
- Inquire about available capacity within HPE Synergy
- Add or remove additional Master/agent nodes to your existing Enterprise DC/OS clusters
- Inquire status on the addition/removal of nodes to/from clusters

Native integration with DC/OS with the dcos CLI enables administrators to add or remove capacity on demand to/from an existing DC/OS cluster. The integration is almost self contained with the only additional infrastructure being an HTTP file server which serves the DC/OS install bits. 

 A single command from an administrators console is all it takes. 
 
```
 $ dcos hpe-oneview --addnode --count=X
```

 The commands supported are as follows
 
 ~~~~
 Usage:
    dcos hpe-oneview --info
    dcos hpe-oneview --alive
    dcos hpe-oneview --help
    dcos hpe-oneview --status
    dcos hpe-oneview --capacity
    dcos hpe-oneview --addnode --count=NO_OF_NODES
    dcos hpe-oneview --removenode --count=NO_OF_NODES
~~~~
  
This native integration capability combined with the ability of DC/OS to scale micro services can enable IT to respond to changes to capacity needs in a matter of minutes.

This project demonstrates the capabilities of composable infrastructure and how it can add elasticity to your cluster.

A demonstration of this integration can be viewed at www.mesosphere.com/blog/


