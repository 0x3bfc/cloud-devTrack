# Cloud Computing Development Track Day 5
-----------------------------------------

#Technical Prespective:
-----------------------

Deeper Dive Taxonomy:
---------------------
	1- SaaS
	2- PaaS
	3- IaaS
	
	- Software as a service:
	-------------------------
		
		1 - Independent of device and location
		
		2 - Not Compatible with all browsers
		
		3 - Authorization and integration:
			- Application on cloud has a structure of user levels to authorize additional features 
			for specific users 'Master Users'
			- The same web interface is used for managing the rights of users
			- Not every SaaS application has to have it's own database of users. 
		
		4- Application integration:	
			
			  Some SaaS apps still needs connections to other applications
			  by copying datasets and using online web services.
			  
		5- Application Customization:
			
			  SaaS applications is almost  by definition multi-tenant, where all users share the same 
			  application, same databases. customization is used to add new features/plugin/web-services.
			  provider has to be sure that any customer cannot access information from another customer.
		
	Platform as a Service:
	----------------------
	
		1- Spectrum:
			
			spectrum of these service is very broad:
			
				- Narrow such as a postal code lookup srvice
				- dedicated domain such as CRM database
				- general purpose such as MS Azure, Google AppEngine, Hadoop
		
		2- Web Service:
														HTTP GET/POST
				User <---> Browser <------> Web Server <----------------> Web Servers
															XML/JSON
															documents
			
					-------------		Request			------------
					|	APP 1	|---------------------->|	APP2	|
					|			|		Response		|			|
					|			|<----------------------|			|	
					-------------						-------------
		
		3- Rich Internet Applications:
		
				The web pages retrieves data using AJAX (Asyncrounce) where communications made in background
		
		4- API and Authentications:
			
				using PaaS to authenticate using Oauth protocol

				
	Infrastructure as a service:
	-----------------------------
		
			- Virtual Machines
			- Content Distribution Networks
			- Storage
			- Cloud Management provider
			
			Virtual Machines:
			-----------------
				
				this layer represent Server Virtualization 
			- Create virtual server
			
			Content Distribution Network:
			-----------------------------
				- situation without a CDN notice that every user gets his data direct from central location
				
					CLOUD -------------CDN1--------ROUTERS-------User1
						|
						----------------CDN2------------ROUTER---------------User in a different location in the world
						
				CDN is used to cashe/buffer the content to provide reliable connection with cloud users
				
			
			Cloud Based Storage:
			--------------------
				1. Storage is essential to IaaS, Servers won't run without it.
				2. Storage can be offered in all three service models
					- IaaS volumes can be attached to servers (Amazon, EBS)
			
			Virtual Appliance and Image Manufacturing:
			------------------------------------------
			
				Provisioning			Manufacturing		Components
				-----------------------------------------------------------
				Community		--->					-->	REDHAT+SYBASE
				ISVs			--->					--> 'Combined Options'
				SI's 			....
				Teams			
				people
				More....		
				-----------------------------------------------------------

		
		Cloud Management and Auditing Services:
		----------------------------------------
			Performance ----------> Cost ----------> Security ------>
					|												|
					Service Orch<-------Configuration	<------------
					
		Networking:
		-------------
			Locations
			Bandwidth
			Latency Tolerance
			Firewalls and Access Control
			Resilience Redundancy
		
		Automation and self-service:
		----------------------------
		
			Traditional ----> self-service ---> Automation 
			
			weeks				days				mins
		
		Federated Identity:
		--------------------
		
		
			Identity provider1				Identity provider1
			Twitter ----------------------------Facebook
				|									|
				----------------|--------------------
								|
								OpenID or Oauth
								
				SaaS Provider 1  Relaying Party   SaaS provider2
				
				
		
		Roles of Standards:
		--------------------
		- Data Format
		- Data Storage
		- Standard VM images
		- Standard Management API
		- Identity Information Standards
		
			
		Chanllenge and Risks:
		----------------------
					- Application performance.
					- Cloud Storage
					- Data Replication alternatives
						- Replication 
						- Synchronize
						- Real-Time lookup
					- Network Security
					- Implication for applications:
					
						Tradition multi-tier:
						---------------------
						- Presentation service "Front-end interface"
						- Business logic Services "Back-end services"
						- Database service
								+
						- Common Services

		Development  Process:
		---------------------
		
			 Cloud computing changes the landscape
				- large ecosystem to draw from
				- Non-functional requirements more easily met
				- changing risks, New risks
			 
			 Instead of design build and order hardware:
				- configured on existing services
				

