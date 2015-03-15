# Cloud Computing Development Track Week 2 - Day 1 
-------------------------------------------------

Adopting cloud computing:
-------------------------
	
	- Roadmaps
	- vendor relation
	- cloud readiness
	- migration applications
	
	
	Roadmaps:
	----------
		
			1- what influences the roadmap?
				- IaaS:
							by upgrading infrastructure or outsourcing
							it is supposed to take first step as a private cloud
							to merge your infrastructure and IT team to be adapted with cloud culture.
							
				- PaaS:
							Using Databases 
				- SaaS:
							something like share-point used locally and used daily.
							
			2- which applications would make a good cloud pilot?
			
				
			3- what pitfalls are there to worry about?



		Factors affect roadmap:
		-------------------------
			They need to rehabilation 
				1- people
				2- products
				3- partners
				4- IT providers
				5- Process
				6- Skills

		- Starting Positions:
		---------------------
			Do not do that :
				- there is a single good level of cloud adoption ----> it is based on your needs
 				- cloud adoptions eliminates all internal IT --------->
 				- Only a handful of cloud providers remain.
 				- the IT department can safely ignore the cloud.
 				
 		
			Nowadays, applications focus on integrations among each other
			
		- Disruptive Technology:
		------------------------
			- Much cheaper
			- Not as good
			- Rapidly imporving
			- Examples: PC, Internet
		
			How to take advantage?
			----------------------
				- find high value, low risk applications 'How to choose pilot?'
				- learn the leasons
		- Types of Organizations most affected:
		---------------------------------------
			- Small office
			- Medium sized enterprises with internal IT dep.
			- Enterprises that deliver IT services themselves
			
		- Application selected:
		-----------------------
			Suitable applications:
			----------------------
			- development and testing apps
			- business continuity:
			
							BCP (Business continuity plan)
										|
										|
								IT Continuity by using DR (disaster recovery) 
			
			- batch and data intensive apps
			- peak load apps
			- desktop apps
			- community SaaS apps
			
			Less Suitable Applicaitons:
			----------------------------
			- legacy applications
			- mission critical apps
			- marginal apps
		
		- Adopting Service Models:
		--------------------------
			1- Private IaaS cloud :
					- Pool some existing servers or acquired IT resources
					- Create standard service catalog
								
						------------------------------------------------
										Service 1
										---------
											|
								----------------------------
								|			|				|
								Service3	Service2		Service4
						-------------------------------------------------
										|			|			|
										X1			X2			X3
					
								
					- Provide user access and chargeback
						- self service
						- metering
						- auto-expire VMs
				
			2- Private PaaS cloud:
			
			3- Is A private SaaS strategy thinkable?
			
				Yes
		- Vendors relations:
		--------------------
			Tiers of Vendors
			-----------------
					1- Cloud Provider				2- Cloud Carier			3- Cloud Consumer
						IaaS
						PaaS							Internet/VPN
						SaaS
													4- Cloud Auditor
													
			Vendor and Provider Dependancies:
			---------------------------------
			
				- Ownership of Hardware and software moves to service provider
				- service disruption causes more immediate impact
				- contingency plan and risk management is necessary.
			
			Vendor Risk management:
			-----------------------
				Depending on the service and deployment model:
					- Data in storage at service provider
					- Images of virtual machines
					- software and software packages
					- machine capacity
					- cloud management tools
					
			Risk Management and cloud migration:
			------------------------------------ 
				- DR
				- Data redundancy
				- Connections redundency 'carier redundency'
			
			Cloud Rediness
			
			Operating Model:
			----------------
				- Process
				- Configuration
				- Technology
				- people
				- Ownership
				
					- Roles and Skills
					------------------
						- Empolying sevice oriented archtichture
						- Evaluating applicability of cloud service models
						- SLA
						- Configuration, integration, and prvisioning of services 
						- Manageing workloads
						- undrastand performance charcterastics
						- Manage security, access protections
					
					- Critical Success Factors
					---------------------------
						1- Vision
						2- Operating Model
						3- Execution of vision and model
						4- continous Evaluation
						 
					- Maturity levels: 5.3.6
		Migrating Applications:
		------------------------
			- Migration Approaches:
			-------------------------
				Migrate mirror exit strategies, how do you move from your current platfrom
					- IaaS approach
					- PaaS approach
					- SaaS approach
					
				
# Operating Cloud Computing:
----------------------------
	"How to manage a service"
	
	1- Impact on service management processes:
	------------------------------------------
		Service Managemet types:
		------------------------
		1- ITIL 'Life cycle of a service'
			- Service startgy
			- service desgine
			- service transition:
					Change of process such as Financial management 'Bugeting, charging, and charge-back'
			- service operational
			--------------------------> continous service improvement
			
			Change Management: 
			------------------	
				RFC 'Request for change'
					- Evaluation			------> CAB	Change Advice Board
					- Authorization			--->	CAB
					- Scheduling 
		
							Change of process
								|
				---------------------------------
				|				|				|
				standard		Normal			Urgent
				low risk
		
		2- MOF 'Microsoft Operation Framework'	
		3- ISO 20K service management processes
			- transition is one of the most important part of service managemet.
	
		Capacity Management:
		---------------------
				capacity management of resources is based on the business needs and demand management.
				by studing the business pattern.
				
				i.e
				
				Service Provider 'Based on demand'			Capacity not assets:
					- Licenses								-------------------
					- HW Assets								- Bandwidth = 300
					- Influence based on 					- Storage = 50 TB
						business pattern					- RAM = 2 TB
						i.e Azure and RHEL					- CPU	....
						if Azure demand increased			Request represented by capacity 
						provider add new features 
						to RHEL to affect on
						business pattern					Request is based on demand.
	
		KPI 'Key performance indicators' for :
			- User Experience
			- Application (transaction volumes)
			- Infrastructure components (utilization)
		
		
		Service Strategy : 
		------------------
		
			Service portfolio Management:
			-----------------------------
			- it consists of service catalog
			- vision 
			- service types
			- compatators
			- edge and advangments
			- it is a document describes all service levels and concepts
			- aceptable risks 'risk appetite'
			- Provisionng from the cloud:
				- matching demand
				- the IT department brings value
				- Financial commitments
			- Desgining chargeback systems:
				- major principles is desgining crosscharging system for cloud computing
						- conform industry norms
						- tie 
						.....
						
			Request Fulfiment:
			-------------------
				- Incident Management .... it is an issue not new request such as service of help desk in organiztion ITIL V2
				- not all requests supposed to be incident, it may be a request 
					such as creating new account for new employee, it is a request fulifiment 'New Request'
				- automated system to change service 'it is a request fulfiment not incident'
		
						Service 1				Service 2					Service 3	........
						----------				----------					---------
							|						|							|
							-----------------------------------------------------
												|
												|
											Unified portal
											---------------
												|
										--------------------------
										| 				|		|
										User 1			User2	User3
			Change Management:
			------------------
					- procedures describes managemnet of changing VMs, DBs, OS ....
					- RFC 'Request for change'.
			
				CMDB 'Configuration management database':
				-----------------------------------------
					- CIs Configurable Items, that needed to be changed 
						- Servers
						- Desktop
						- printers
						- Operating system
						- App1, .. App2
						- developer 1 ..., developer2
						- customer support 1 , .... customer support 2 ..
							
						For examples:
							service 1 : needs printer + server2 + Operting system ...
							where you know where the relations between service and components of your system
						
# Govern the Cloud:
-------------------

	- Risk Managements:
	-------------------	
		The proactiive identification analysis and control of risk which can threaten the 
		assets  or the earning capacity of an enterprise.
			
			First you have to detect the risk then apply analysis on it.
			
			Risk (Threat):
			--------------
				- Avoid  (avoid business opportiunity)
				- Fallback (is based on impact, low probablilty )
				- Reduce
				- Accept (accept the risk)
			
			Analysis:
			---------
					- Probability 			Impact of risk
						High					High			(AVOID)
						low						high			(FallBack)
						high					low				(Reduce)
						low						low				(Accept)
					
			based on analysis, we add the priority of solutions 
	
			ACCEPTABLE RISK
			---------------
			Risk action can not eliminate the risk, but still exists some of risk residual
			by adding another risk actions to get the acceptable risk
			
			Inhrideted risk
			---------------
				it is risk nested risk
	
		- Compliance
		
		- In-house system management versus cloud computing:
		
				Pros												Cons
			using IaaS may, infact be beneficial in your
			change management process
			cloud service prviders build in 
			features to accommodate clients 
			release schedule.
	


		- Security
			- insecure communication
			- multiple touch points
			- attach approaches
			- social engineering
			
		- Residual risks

		- Privacy
			- between stackholders and party.
			- confidentiality of data.
		
		- Jurisdiction
			- who can look at email that is stored at a cloud provider? 
		- Data protection directives
		- Reputation
		- Legal
			Service level agreement
				- Type of functionality offered
				- percentage of gurenteed uptime
				- response time
				- financial paragraph
			most of legal and financial topics are covered in contract
		- Licensing
		- Activity:
			- Identity management vendor (IDM) control the user's identity
			- control the number of concurent users in the client organization
		

#Financial Management:
---------------------
	- Management measures
		- Direct costs 
		- cost allocation
		- Role-play
# Strategic Supplier Management:
--------------------------------

		- Exit strategy:
		----------------
				- Business close by the vendor
		- Strategic Options:
		----------------------
			- outsource business process
			- different applications (saas/in-house)
			- rehost (IaaS/ In-House)
			
