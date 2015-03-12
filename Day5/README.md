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
				
				this layer represent Server Virtualization 
			- Create virtual server
			
