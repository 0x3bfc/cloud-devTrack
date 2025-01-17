CLOUD COMPUTING DEVELOPMENT (DAY 5 WEEK3)
-----------------------------------------
	
# Module 7 Service Operation
-----------------------------

	
		Service Operation functions:
		----------------------------
			- The service Desk 
			- Technical Management 
			- Application Management 
			- IT Operations management
			
		
		1- Event Management:
		---------------------
			Event:
				an alert is a message generated by a device when an event occured and generated by Event management system.
				
			- such as Event Logs (Input), detect all changes of state that have significance for management of a 
			  configuration item 
			- Management events through their lifecycle
			- coordinate the activities to detect events, make sens of them and determine the appropriate control action 
			- Event Manegment detects and monitors the service's components and configration items
			- Scope:
				- Change management
				- Normal Activity
				- Enviromental conditions 'automation of some machines with specific environmental conditions'
				- security level 
				- software licenes
			- Event types:
			--------------
				- Exceptions
				- Normal or informational 
				- warning
			
			
		2- Incident Management:
		-----------------------
			Incident:
				is an unplanned interruption or a reduction in the quality of an IT service, or anything 
				may affect an IT service in the future "Quota" (Proactive incident)
			Timescale:
				- The time to resolve this incident
				- Supported tools must be a ware of the timescales 
			
			Escalatation: 
				- functional escalation (need more knowledge/experience) 
						Service Desk ----> First Line Support ----> Second Line Support 
						
				- Hierarchical Escalation (up to the management chain)
						Service Desk ---> Not supported as Technical solution
								---> move to business or management to decide strategic solution
								
			- Purpose:
				- restore normal service operation ASAP
				- minimize the adverse impact on business operations
				- ensure that the agreed levels of service quality are maintained
			
			it is used to standardize the methods and procedures are used reporting incident 
			
			- Scope:
				- Service Desk (Users submits incidents)
				- Event Management (Exceptions)
				
			Priority:
			---------
				is based on impact and urgency
					- Impact:
						measure of the effect of an incident on business
					- Urgency: 
						is a measure of how long it will be untill an incient , a prplem has a siginificant impact 
					on business
					
				Priority = Impact x urgency
				
			Incident Model:
			---------------
				- steps to handle the incident
				- roles and resp.
				- time scales 
				- escalation proceures
			Interfaces:
			-----------
				- ISM
				- PM
				- CM
				- SACM
				- AM
				- CM
			page 468
						
											Event Management  ..... 
												|
											Incident identification
												|
											is this really an incident
												|
											incident logging
												|
					Major incident procedure<---Major incident
													|
												Initial Diagnosis
								yes				yes	|
					Functional---- Functional<----Escalation Needed
					Scalation		Scalation				|
										|		investation and diagonsis?
					Management<-----Hierachic 			No	|
					Scalation		Scalation				|
												Resolution and recovery
															|
														Incident closure
															| 
														   end
				
			Notes:
			------
			- exceptions in events used as incident that would be as a problem for incident management department 
			
		3- Request Fulfilment:
		----------------------
			processes responsible for managing lifecycle of all srvice request form user
			
				- Ensuring user and customer satisfaction through efficient and professional handling of problem
				- sourcing and delivering the components of request standard services 
			Scope:
			------
			
			Service Request:
				- Information
				- advice
				- standard change
			No suported
			-----------
				- RFC 'Request for change' submitted to incident management
		4- Problem Management:
		----------------------
	
			A problem:
			----------
				is the cause of one or more incidents, where the cause is usually not know as the time
				a problm record is created
					
					Lifecycle of problem:
					----------------------
					
					repeated incident ---> Problem -----> Know Error ------> Know Error with work around ---> Record in 
																										Knowledge management system
	
			- repeated incidents have the same characteristics
			- managment of all lifecycle of all problems 
			- detect the root cause of incidents 
			- define the root cause, document, communication known errors and inciate actions to
			  improve actions or correct situation
			
					Problem Management
							|
							|
				------------------------------
					|					 |
				Reactive				Proactive
				solving 				indentifing
				problem					improvment
		
			Interfaces with problem management:
			-----------------------------------
						- Service Design
						- Service Strategy
						- Service Transition
						- Continual service Improvements
			Activities:
			------------
				page 469
		
		5- Access Management:
		---------------------
			Ensure that access is granted to users according to information security policy, also some services 
			provides single point of contact 'portals' and monitoring the access.
		
			Access:
				The level and extent of a service functionality or data that a user is entitled to use
				
			Identity:
				Information about users that distinguishes them as inviduals and verifies their status 
				within the organization.
			Right:
				Privileges, or rights refer to the actual settings where user is provided to 
				access to a servcice or group of services.
		
		 types of acess services:
		 ------------------------
			- service or service groups
			- Directory services
		
# Service Operation Functions:
------------------------------
	1- The service Desk Function:
	-----------------------------
		- Functional unit to deal with variaty of service events by ensuring that it single point of contact for all requests
		- Mapping requested and incident to specialists and return the output to sender.
		 types:
			1- Local service desk
			2- centralized service desk
			3- virtual service desk:
			
		Structures:
			- follow the sun
			- specialized service desk
		Roles:
			- The service desk manager
			- Service Desk supervisor (Optional)
			- Service Desk analyst (First level support for IM 'incident management')

	2- Technical Management Function:
	----------------------------------
		Units:
			1- Network dep
			2- Database dep.
			3- storage dep.
			4- Directory service dep.
	
	3- Application Management Function:
	-----------------------------------
		- supports and maintains operational application services.
		
		- roles:
		
			- Application manager:
				- Financial application 
				- HR application
				- Business application
		Application Development ---> Design Issue (Requirement --> analysis --> Design --> Implementation ---> Testing)
		Application Management ----> Operational Issue
	
	4- IT operational Function:
	----------------------------
		responsible for daily operational activities needed to manage the IT infrastructure
		
		Role:
			IT operations control:
			-----------------------
			- console management
			- print and output
			- job scheduling
			- backup and restore
			Facility Managment:
			-------------------
			- Data centers
			- recovery sites
			- consolidation 
			- contracts
	


# Module 8 Continual Service Improvement (CIS):
-----------------------------------------------
	
	- Providing giudance on creating and maintaining value for customers
	- combines principles, practices methods from quality management
	- Ensure that the service portfolio continues to be aligned to business needs
	- includes service measurement, demonstrating value with metrics, 
		develeping baseline and maturity assesments
	
	Continual Service Improvement Lifecycle:
	----------------------------------------
		dependes on identifying and using improvements opportuities 
		througout the entire service lifecycle
	
		- Get feedback from all processes across services.
			Page 277
		- CSI register used for improvement actions and plans
			"You can improve, you can measure"

		CSI:
		----
			- Contains a clear prioritized list of items where improvements can be made
			- keeps records of all improvement opportunities 
			- has categories of initiatives that can be achieved quickly
		
	The Deming - PDCA cycle:
	------------------------
	
			- Plan ---> Do ---> Check --> Act
				|							|
				<----------------------------
			- The maturity of service is increased by improving the service over Deming cycle
			  to align business need 
	
	Models of CSI:
	--------------
				1- CSI approach:
					 						What is the vision?				Business vision and missions
											
											Where are we now?				Baseline assessments
									
					How do we keep 			Where do we want to be?			Measurable target
					the momentum going? 	
											How do we get there?			Service and process improvement
												
											Did we get there?				Measurement and metrix
				
						
	
				2- Key Performance Indicator (KPI) and ciritical success factor CSF 
					it is used for measurments
					- identify the right critical success factors based on the objectives of processes
						i.e users are replying emails for specific service we offers not the users that get my ads
					- ensure that they adopt key performance indicators KPIs after careful considration
				3- Baseline
					marker or start points for comparing later imporvements 
	Types of Metrics:
	-----------------
		- Technology metrics 
		- Process metrics 
		- Service metrics
	
	Seven Steps improvements process:
	---------------------------------
		1- identify
		2- define
		3- gather
		4- process
		5- analysis
		6- present
		7- implement
	
# Module 9 Technology and Architecture:
--------------------------------------

		- Service Automation 
		- Competence and skills for service management
		
	
