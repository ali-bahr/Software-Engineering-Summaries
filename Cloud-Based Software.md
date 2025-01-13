#### **1. Introduction to Cloud Computing**

- **Definition**: Cloud computing involves renting remote servers hosted by companies (e.g., AWS, Google Cloud, Microsoft Azure) to run software and make it accessible to users over the internet.
    
- **Key Characteristics**:
    
    - **Scalability**: The ability to handle increasing numbers of users while maintaining performance.
        
    - **Elasticity**: The ability to scale resources up or down based on demand.
        
    - **Resilience**: The ability to maintain service in the event of server failure.

#### **2. Benefits of Cloud Computing**

- **Cost**: Avoids upfront capital costs for hardware.
    
- **Start up Time**: Servers can be set up in minutes.
    
- **Server Choice**: Easily upgrade or downgrade server resources.
    
- **Distributed Development**: Teams can work from different locations with the same development environment.

#### **3. Virtualization**

- **Virtual Machines (VMs)**:
    
    - Simulate physical servers using a hypervisor.
        
    - Run their own operating system and software.
        
    - Suitable for isolated environments but slower to start and stop.
        
- **Containers**:
    
    - Lightweight virtualization technology that shares the host operating system.
        
    - Faster to start and stop compared to VMs.
        
    - **Docker**: A popular container management system that allows defining and running containers using Docker images.

#### **4. Docker**

![[Pasted image 20250113103105.png]]

- **Docker Components**:
    
    - **Docker Daemon**: Manages containers on the host server, used to setup, start, stop, and monitor containers, as well as building and managing local images.
        
    - **Docker Client**: Used by developers to define and control containers.
        
    - **Dockerfile**:
	    - Defines applications (images) as a series of setup commands that specify the software to be included in a container.
	    - Each container must be defined by an associated Dockerfile.
        
    - **Docker Image**: A runnable application created from a Dockerfile.
        
    - **Docker Hub**: A registry of Docker images for reuse.
		
	- **Containers**: 
		- Containers are executing images. An image is loaded into a container and the application defined by the image starts execution.
		- Changes to a Docker container (e.g. by modifying files) must be updated by committing these changes to create a new image and restart the container.
        
- **Benefits of Containers**:
    
    - Solve software dependency issues.
    - Enable software portability across different clouds.
    - Simplify DevOps practices.


#### **5. Everything as a Service (XaaS)**

- **Infrastructure as a Service (IaaS)**:
    
    - Provides virtual servers, storage, and networking.
        
- **Platform as a Service (PaaS)**:
    
    - Provides development frameworks and tools.
        
- **Software as a Service (SaaS)**:
    
    - Delivers software over the internet via a subscription model.

#### **6. Software as a Service (SaaS)**

- **Benefits for Providers**:
    
    - Regular cash flow through subscriptions.
    - Easier update management and bug fixes.
    - Continuous deployment of new features.

- **Benefits for Customers**:
    
    - No upfront costs for software or hardware.
    - Immediate access to software.
    - Immediate software updates.
    - Reduced software management costs.

- **Challenges for Customers**:
	- Privacy regulation conformance.
    - Network constraints (e.g., response time).        
    - Security concerns (e.g., sensitive data).
    - Service lock-in (e.g., difficulty switching providers).

#### **7. SaaS Design Issues**

- **Local/Remote Processing**: Balance between processing on the client side vs. server side.
    
- **Authentication**: Use Own authentication, external authentication (e.g., Google, Facebook) or federated authentication (e.g., Okta).
	
- **Information leakage:** if there is multiple users from multiple organizations you must separate their information.  
	
- **Multitenant vs. Multi-Instance Databases**:
	    ![[Pasted image 20250113111215.png]]
    - **Multitenant**: 
	    - Single database shared by multiple customers. 
	    - Database is partitioned so that customer companies have their own space and can store and access their own data.
		- **Database Customization in SaaS**:
			- **Extending Databases**:
			    - **Extra Columns**: Add additional columns to tables for customer-specific data.
			    - **Separate Tables**: Use additional tables to store custom fields and values.
			- **Security**:
			    - **Multilevel Access Control**: Control access at both organizational and individual levels.
			    - **Encryption**: 
				    - Encrypt data to prevent unauthorized access. 
					- data cannot be viewed by people from other companies if some kind of system failure occurs.
					
		- **Advantages**: Efficient resource utilization, easier updates, security management is simplified as there is only a single copy of the database software to be patched if a security vulnerability is discovered.
            
        - **Disadvantages**: Security risks (data leakage), inflexibility, database security breach affects all customers, increased complexity.
        
        ![[Pasted image 20250113111536.png]]
		
		![[Pasted image 20250113111611.png]]
		
	- **Multi-Instance( Single Tenant )**: Separate databases for each customer.
	    - Each instance of the software can be tailored and adapted to a customer’s needs. 
	    -  Customers may use completely different database schemas.
	    -  Specific systems can be scaled according to the needs of individual customers.
	    - If a software failure occurs, this affect a single customer. Other customers can continue working as normal.
        - **Advantages**: Better security, flexibility, Scalability, Resilience.
            
        - **Disadvantages**: Higher cost, complex update management.
		
		![[Pasted image 20250113111653.png]]


#### **9. Scalability and Resilience**

- **Scalability**:
    
    - **Horizontal Scaling (Scaling Out)**: Add more servers to handle increased load.
        
    - **Vertical Scaling (Scaling Up)**: Increase the power of existing servers.
        
- **Resilience**:
    
    - Use ==redundant== servers and databases in different locations.
        
    - Implement system monitors to switch to standby systems in case of failure.
		
	- Database updates are mirrored so that the standby database is a working copy of the operational database
	
	![[Pasted image 20250113114313.png]]





### **Question Bank**

1. **Which of the following are key characteristics of cloud computing?** (Select all that apply.)  
    A) Scalability.  
    B) Elasticity.  
    C) Resilience.  
    D) High upfront costs.  
    
    **Correct Answers**: A, B, C
    
2. **Which of the following are benefits of cloud computing?** (Select all that apply.)  
    A) Avoids upfront capital costs for hardware.  
    B) Servers can be set up in minutes.  
    C) Limited server choices.  
    D) Teams can work from different locations with the same development environment.  
    
    **Correct Answers**: A, B, D
    
3. **Which of the following are true about virtual machines (VMs)?** (Select all that apply.)  
    A) They simulate physical servers using a hypervisor.  
    B) They run their own operating system and software.  
    C) They are faster to start and stop compared to containers.  
    D) They are suitable for isolated environments.  
	
	**Correct Answers**: A, B, D
    
2. **Which of the following are true about containers?** (Select all that apply.)  
    A) They share the host operating system.  
    B) They are slower to start and stop compared to VMs.  
    C) Docker is a popular container management system.  
    D) They are lightweight and portable.  
    
    **Correct Answers**: A, C, D
    

1. **Which of the following are components of Docker?** (Select all that apply.)  
    A) Docker Daemon.  
    B) Docker Client.  
    C) Dockerfile.  
    D) Docker Hub.  
	
	**Correct Answers**: A, B, C, D
    
2. **Which of the following are benefits of using containers?** (Select all that apply.)  
    A) Solve software dependency issues.  
    B) Enable software portability across different clouds.  
    C) Simplify DevOps practices.  
    D) Require more resources than VMs.  
    
    **Correct Answers**: A, B, C
    
1. **Which of the following are true about multitenant databases?** (Select all that apply.)  
    A) They are more cost-effective than multi-instance databases.  
    B) They pose security risks due to data leakage.  
    C) They are easier to update than multi-instance databases.  
    D) They offer more flexibility than multi-instance databases.  
    
    **Correct Answers**: A, B, C
    
2. **Which of the following are true about multi-instance databases?** (Select all that apply.)  
    A) They are more expensive than multitenant databases.  
    B) They offer better security than multitenant databases.  
    C) They are easier to update than multitenant databases.  
    D) They are less flexible than multitenant databases.  
    
    **Correct Answers**: A, B
    
1. **Which of the following are true about scalability?** (Select all that apply.)  
    A) Horizontal scaling involves adding more servers.  
    B) Vertical scaling involves increasing the power of existing servers.  
    C) Scaling out is the same as vertical scaling.  
    D) Scaling up is the same as horizontal scaling.  
    
    **Correct Answers**: A, B
    
2. **Which of the following are true about resilience?** (Select all that apply.)  
    A) It relies on redundancy.  
    B) It involves replicating software and data in different locations.  
    C) It is unrelated to system availability.  
    D) It can be achieved using standby systems.  
    
    **Correct Answers**: A, B, D





