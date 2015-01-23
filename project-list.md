# Open Source Networking Projects
Brief description of open source networking projects.  This list was originally posted at http://www.jedelman.com/home/open-source-networking.  The goal is to make this an evolving community driven list.  Feel free to issue a pull request to make any change to the existing list or add net new projects.  

**Note: Please keep the descriptions concise and also include a link if you are going to add a project.**

### [OpenDaylight (ODL)](http://www.opendaylight.org/)
Established in April 2013 is an open source Software Defined Networking (SDN) controller platform(s).  There are different controller platforms for different use cases.

### [OpenFlow (OF)](https://www.opennetworking.org/ja/sdn-resources-ja/onf-specifications/openflow)
Established in the late 2000s, the OpenFlow 1.0 release launched in December 2009.  The Open Networking Foundation took over the development (not actually coding) of OpenFlow when ONF formed in late March / early April in 2010.

### [Open vSwitch (OVS)](http://openvswitch.org/)
Established in mid to late 2009 by the Nicira team to replace the standard Linux bridge.  It’s goal was to provide full featured switching capabilities to virtual environments running in Linux based hypervisors such as KVM and XEN.  It’s also now being used to inter-connect containers.

### [Open Virtual Network (OVN)](http://openvswitch.org/pipermail/dev/2015-January/050380.html)
Just established last week and will be a sub project of the OVS project.  Its goal is to provide native abstractions to OVS to simplify the provisioning of logical segments, logical routers, and security groups without requiring a SDN controller (initially for OpenStack environments).

### [OpenStack Neutron](https://wiki.openstack.org/wiki/Neutron)
Formerly known as Quantum, it is the core networking project and API for the OpenStack project.  For networks to be orchestrated by OpenStack, they must have a neutron plug in.  It officially became a core project in the OpenStack Folsom release.

### [OpFlex](https://tools.ietf.org/html/draft-smith-opflex-00)
Launched in early 2014 by Cisco as a way to create, deploy, and manage policies. It’s initially being used as part of the Cisco Application Centric Infrastructure (ACI) solution.  Cisco has also submitted it to the IETF and is contributing work around OpFlex to the ODL and OpenStack Neutron communities.  The OpFlex project consists of three things: the OpFlex protocol, SB plugin, and the policy agent.

### [Data Services Engine (DSE)](https://github.com/stackforge/congress/tree/d1ef962a7e6e1a55537d50ebb3604ade73ba2588/congress/dse)
Initially created in 2013 by Plexxi, the DSE has become part of the OpenStack Congress project (focused on policy).  The DSE could revolutionize how different products and solutions communicate with one another.  I’ll go out on a limb and say it could be the foundation for machine learning in the data center (and IT, more generally).

### [Quagga](http://www.nongnu.org/quagga/)
This one has been around for some time, but is gaining more visibility with companies like Cumulus actively promoting open networking.  Quagga is a routing software suite and has open source implementations of OSPF, RIP, BGP, etc.

### [OpenContrail](http://www.opencontrail.org/)
Juniper acquired Contrail, a network virtualization company, in December 2012.  Shortly after, they open sourced the product and called it OpenContrail.

### [MidoNet](http://www.midokura.com/press-releases/midokura-open-sources-complete-iaas-network-virtualization-solution-openstack-community/)
The network virtualization product by Midokura was just open sourced less than 3 months ago.  Like a few other startups and solutions out there, they have been primarily focused on networking for OpenStack clouds.

### [Open Networking Install Environment (ONIE)](http://onie.opencompute.org/)
Created by Cumulus Networks in 2012 and later adopted by the Open Compute Project (OCP), it is a lightweight operating system serving as a boot loader for bare metal switches allowing users to have choice in which operating systems can be used and loaded.  Cumulus, Big Switch, OCP, Pica8, Dell, and Plexxi (they’ve committed to it, but don’t know where they stand) are now shipping switches with ONIE pre-installed and/or support ONIE in their software.  You can find plenty whitebox/bare metal platforms that ship with ONIE that will allow you to load network operating systems like Cumulus Linux, Open Networking Linux, PicOS, etc.

### [Open Compute Project (OCP)](http://www.opencompute.org/projects/networking/)
Has been around since 2011 initially established by Facebook to share some of their hardware designs, but also to help accelerate hardware and software innovation in the open source world.  OCP Networking was later established in early to mid 2013, publicly launched at Interop in 2013.  It’s since been working on open source architectures for data center top of rack switches.

### [Prescriptive Topology Manager (PTM)](http://cumulusnetworks.com/blog/complex-topology-and-wiring-validation-in-data-centers/)
Created by Cumulus in 2013 as a way to dynamically verify there is up to date and accurate cabling in place in switched networks.  This is great and I do hope other vendors adopt PTM.  I’ve been developing external (off box) functionality to do the same thing.  Check out my blog for more details.

### [Open Networking Linux (ONL)](http://opennetlinux.org/)
Emerged onto the scene in late 2013 by Big Switch Networks and is now part of the Open Compute Project (OCP).  ONL is a base level Linux distribution for bare metal switches.  One of its main goals is to be the foundation of which others/vendors can build commercial solutions on top of bare-metal switches.  Big Switch’s SwitchLight OS is an example, and is built on top of ONL.

### [Bird Internet Routing Daemon (BIRD)](http://bird.network.cz/)
Similar to Quagga, it is an open source routing platform for Linux systems.  In contrast to Quagga, BIRD offers multiple-RIB design, is often used as a route server, and does not support ISIS.  On the other hand, Quagga is a single-RIB design, supports ISIS, and it’s not even recommended to be used as a route server.

### [Snort](https://www.snort.org/)
Many are aware of Snort, but it’s an open source IDS/IPS; its commercial version came via SourceFire, a company which Cisco acquired in 2013.

#### There are plenty more open source projects that will directly impact networking too.  A few of them include:

#### [OpenFlow controller](http://yuba.stanford.edu/~casado/of-sw.html)
There are plenty of these still out there, many in academia

#### [Git](http://git-scm.com/), [Gerrit](http://code.google.com/p/gerrit/), [Jenkins](http://jenkins-ci.org/), [Travis CI](https://travis-ci.com/)
Open source tooling for source control, code review, testing, and continuous integration.  These aren’t too popular in the network community, but they can definitely have a positive impact.

#### [SocketPlane](http://socketplane.io/), [Weave](http://weave.works/), [Akanda](http://www.akanda.io/)
New onto the network scene, SocketPlane and Weave are building open source networking solutions for Docker and Akanda (spin out from Dreamhost) is building an open source network virtualization platform for OpenStack environments.

#### [Ansible](http://www.ansible.com/home), [Puppet](http://puppetlabs.com/), [Chef](https://www.chef.io/), [SaltStack](http://www.saltstack.com/), etc.
Here is an increasing amount of open source automation and configuration management tools that have been around for quite some time, but we’re just starting to see what kind of impact and what the integrations will look like for the network community

And we can’t forget about [OpenNMS](http://www.opennms.org/), [Zenoss Core](http://www.zenoss.org/), [Nagios Core](http://www.nagios.org/projects/), etc.  If you want to add more to this list, feel free to write in or comment below.  
