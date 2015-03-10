Cloud Computing Development Track Day 3 (VEP) Cont.
----------------------------------------------------

KVM (Cont.)
-----------

	Shared Memory virtualization

		KSM stands for Kernel same-page merging where the hypervisor system share identical memory pages amongst different processes or 
		virtualized guests. While not directly linked, KVM can use KSM to merge pages of Virtual machines.




Application Virtualization:
---------------------------

		Containers vs VMs
		

		VM1		VM2		VM3				APP1	APP2	APP3  APP4	
		--------------------			--------------------------
			Hypervisors					CONTAINER ENGINE 'DOCKER'
		--------------------			---------------------------
			HOST OS								HOST OS
		--------------------			---------------------------
			HARDWARE							HARDWARE
		--------------------			---------------------------
		
		
		Linux Container:  LXC is an operating-system-level virtualization environment for running multiple isolated Linux systems (containers) on a single Linux control host.
		
		
					--------------------------------
					|Container 1 | Container 2 | ..|
					--------------------------------
					|		LXC-Docker			   |
					--------------------------------
					| Kernel 'Namespaces'+'cgroups'|
					--------------------------------
					
			- Linux Kernel uses kernel module called 'cgroups' or control groups to manage the hardware resource isolation such as 
			(CPU, memory, block I/O, network), and application isolation using another kernel module 'NameSpaces'. 
			- LXC provides the operating system level virtualization that has its own process and network space, 
			instead of creating a full-fledged virtual machine.
			- But container technology is less secure than full OS virtualization  
			
			
		Container Technologies: 
			- LXC
			- OpenVZ
			- Docker
			- Linux Vserver



	Notes:
		- Check Operating System level virtualization table http://wikipedia.org/wiki/Operating-system-level-virtualization
		- Copy-on-write (sometimes referred to as "COW") is an optimization strategy used in computer programming. The fundamental idea is that if multiple callers ask for resources which are initially indistinguishable, you can give them pointers to the same resource.
		
		

Network Virtualization: (Cont.)
-------------------------------

		- Access Control List: 
					provide secure, customized access for individuals and groups to protect enterprise lan from
					external threats by droping any user does not have access for this network. include the following:
									1- source ip
									2- destination ip
									3- address protocol
									4- source port
									5- destination port
								Examples:
										1- Network Access Protection (NAP)
		- Path isolation:
					use a mix of layer 2 and layer 3 technologiess to best address LAN virtualization for typical LAN desgine 
					Examples:
							1- VLAN
							2- VPN	"Encrypted tunnel between more than one network that are separated phyically over internet"
							3- MPLS "multi-protocol label switching" by using router/nodes labeling
									 is a mechanism in high-performance telecommunications networks that directs data from one network node to the next based on short path labels rather than long network addresses, avoiding complex lookups in a routing table.
							4- VRF  "virtual routing and forwarding"

		- Virtual service: virtual Firewall  WAN Optimization.
		
		- Open Networking Open Source: Network tools
					
					1- Altor network virtual firewall provide policy based firewall protection for virtual machine as well as an 	
										intrusion detection that offers traffic scanning and alerting on virtual switchs. 
					2- vyatta virtual router
					3- Open vSwitch 
					4- OpenStack "Private Cloud Network virtualization 'neutron'"


Desktop Virtualization (Cont.)
-------------------------------

		Workspace virtualization technology
	
		- Terminal services multiple user can access application that are hosted on the same operating system
		- VDI Virtual Desktop Infrastructure: works by attachments user data , application send the operating system from the end point device i.e laptop using 'rdesktop' and desktop using thin client

		Advantages:
			- more secure
			- simple administration
			- more reliable
			- application streaming

Storage Virtualization:
-----------------------		

	Types of Storage virtualization:
	
		- Block virtualization
		- File system virtualization.
		
	Types of storage:
	
		- Enterprise Storage
		- locally attahced storage
		- SSD
		- SAN
		- NAS
		- Storage Array
		- Tapes
		- removable storage
		
		BLOCK VIRTUALIZATION
		---------------------
				- Address space remapping: 
									virtualization of storage provides the location indenpendent solutions. it support lgical
									space for data storage and handles the processes of mapping them to actual physical storage.
				- Meta-Data:
									The mapping information for the virtualized storage called meta-data that needed to be managed
									and maintaining a consistant view of data.
				- I/O redirection:
									The virtualization software or device uses the meta-data to re-direct I/O requests. It will 
									receive an incoming I/O request containing information about the location of the data in terms of 
									the logical disk (vdisk) and translates this into a new I/O request to the physical disk location.
									Ex. Perform a meta-data look up for LUN ID=1, LBA=32, and finds this maps to physical LUN ID=7, LBA0
				- Replication:
									When storage is virtualized, replication services must be implemented above the software or 
									device that is performing the virtualization. This is true because it is only above the 
									virtualization layer that a true and consistent image of the logical disk (vdisk) can be copied. 
									This limits the services that some implementations can implement - or makes them seriously 
									difficult to implement. If the virtualization is implemented in the network or higher, this 
									renders any replication services provided by the underlying storage controllers useless.

				- 
