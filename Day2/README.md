Cloud Computing Development Track Day 2
----------------------------------------
9-3-2015

Hypervisors structure:
----------------------

	USER SPACE <APPS>
	Kernel Space
	HW. Emulator
	
Tools for virtualizations:
--------------------------

	1. KVM 
	2. Xen 
	3. VMware
		
			- Vsphere	
			- VMware workstation
			
	4. RedHat	RHEV
	5. Windows	Hyper-v



Vendors:
--------

		- VMware
		- CITRIX
		- RedHat
		- Microsoft
		
Types of Virtualization:
========================


1- Fully Virtualization 
		
				---------------------------------
				| Guest	| Windows | Linux OS| ..|
				----------------------------------
				|		| 		HyperVisor		|
				---------------------------------
				|		|		Kernel 			|
				|  HOST	-------------------------
				|		| Physical Hardware		|
				--------------------------------

			 Advantages:
				- able to run over any operating system
			 disadvantages:
				- lower performance due to using the hiegest number of virtualization stack
				
			 Examples:
					VMware Workstation


2- Para Virtualization

			------------------------------------
			Guest OS | Guest OS ...
			------------------------------------
			Hypervisor
			------------------------------------
			Share Xen Kernel for all Guest OSes
			------------------------------------
			HardWare
			-------------------------------------
			
			
			in para virtualization all OSes in para share the same kernel in case of Microsoft Windows uses the full
			stack virtualization

			- XEN Kernel:
				- disadvantages --- specific linux kernel, where kernel limitaions.
			- XEN citrix: provides XENServer, XenDesktop
			
			
3- kernel virtualization

			- KVM: Enable Hypervisor operation in linux kernel, where KVM provides the 
					virtualization layer on the same kernel of Host OS
			
			
			------------------------------
			VM1 "APP + Kernel" | VM2 | VM3
			------------------------------
			KERNEL
			------------------------------
			Physical Hardware
			------------------------------
			
			- Technologies: RHEV "RedHat Enterprise Virtualization"
							VMware-Vsphere and V-cloud
							

Types of Hypervisor:
--------------------

Type 1 : Bare-Metal Hypervisor

			-----------------------------------------------
			| OS1 | OS2| .................................| 
			-----------------------------------------------
			|			Virtualization Layer			  |
			-----------------------------------------------
			| X86 Architecture "CPU + RAM + NIC + Storage"|
			-----------------------------------------------

		1- VMware ESX and ESXI has a management tool called Vcenter
		2- RHEV-H	has a Management tool called RHEV-M
		
				-----------------------------								 -----------------	
				|H1|		|H2|		|H3|	Hypervisor servers --------> | SHARED STORAGE|		
				-----------------------------								 ----------------- 	
				  |			 |			 |
				  |----------------------|
							|
					---------------------
					|	Management Tool |		Management Server
					---------------------									-------------
							|-----------------------------------------------|	Client 	|
																			-------------
				
				- Better performance for virtual machine provisioning
				- support live migration for from strugglers Hypervisor server to another.
				- But for live migration, all virtual machine must be shared on the same physical storage
				  to be enabled, they use the meta data of virtual machine on shared physical storage 
				  to start any virtual machine and balance the load over hypervisor servers.
				- this type of virtualization supports the high availability and data consistancy of service. 


		Live Migeration:				-------------STORAGE---------
										|							|
					|Guest OS1|	|Guest OS1|				|Guest OS1||Guest OS1|
					-----------------------				----------------------
					|	HyperVisor 1	  |				| Hypervisor 2		|
					-----------------------				----------------------	

			- Failure Detector: User specify in configurations how to detect the Virtual Machine Failure to migrate the VM from H1 to 
			  H2 and vice versa.
			- Provide Fast Recovery time with minimal down time.

		Storage:
		
				1- Backup: by cloning virtual machine 'Full backup' the same size of the source Virtual machine
				2- Snapshot: copying of data index but the data still exists, if there is any change (Edit/Delete/Add) in file  
				   system, copy this change to snapshot, to keep track all changes in file system 

			
Type 2: Hosted Hypervisor

			-------------------------------------
			|		|	Guest OS | Guest OS	| ..|
			|	APP	-----------------------------
			|		| Virtualization Layer		|
			-------------------------------------
			|		Physical Hardware			|
			-------------------------------------

Notes:

		Hardware assistance:
	
			improve performance and support virtualization of DMA I/O and memory virtualization 
			for example VT-x and AMD-V started being introduced into CPU desgins in 2005


Network Virtualization:
-----------------------


			
			
