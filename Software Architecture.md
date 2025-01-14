#### **1. Introduction to Software Architecture**

- **Definition**: Software architecture refers to the fundamental organization of a system, including its components, their relationships, and the principles guiding its design and evolution.
	
- **Importance**: Architecture significantly influences non-functional system properties like **performance**, **security**, **reliability**, and **maintainability**.
    
- **IEEE Definition**: Architecture is the fundamental organization of a system embodied in its components, their relationships, and the principles guiding its design and evolution.

#### **2. Non-Functional Attributes**

- **Responsiveness**: Does the system return results to users in a reasonable time?
    
- **Reliability**: Do the system features behave as expected ==always== by both developers and users?
    
- **Availability**: Can the system deliver its services when requested by users?
    
- **Security**: Does the system protect itself and users’ data from unauthorized attacks?
    
- **Usability**: Can users access and use system features quickly and without errors?
    
- **Maintainability**: Can the system be updated and new features added without excessive cost?
	
- **Resilience**: Can the system continue to deliver services in the event of partial failure or external attack?


#### **3. Architectural Design Issues**

- **Non-Functional Product Characteristics**: Security, performance, and other attributes affect all users. Some characteristics are opposing, so trade-offs are necessary.
    
- **Product Lifetime**: Long-lived products need architectures that can evolve to accommodate new features and technologies.
    
- **Software Reuse**: Reusing components (e.g., open-source software) can save time but may constrain architectural choices.
    
- **Number of Users**: Systems with rapidly changing user numbers need architectures that can scale quickly.
    
- **Software Compatibility**: Maintaining compatibility with other software may limit architectural choices (e.g., database selection).

#### **4. Architectural Trade-offs**

- **Maintainability vs. Performance**:
    
    - **Monolithic Architecture**: Easier to maintain but may suffer from performance issues.
        
    - **Component-Based Architecture**: Improves maintainability but may introduce performance overhead due to inter-component communication.
        
- **Security vs. Usability**:
    
    - **Layered Security**: Improves security but may reduce usability by adding authentication steps.
        
    - **Usability**: Too many security layers can frustrate users, so balance is key.
        
- **Availability vs. Cost**:
    
    - **Redundancy**: Improves availability but increases development time, cost, and complexity.
        
    - **Time-to-Market**: Adding redundant components may delay product release.
        

#### **5. Component Organization**

- **Abstraction**: Focus on essential elements without concern for implementation details.
- Architectural Level: Large-scale Components
- **Decomposition**: Break down large-scale components into finer-grained components.
- **Layered Architecture**: Organize components into layers (e.g., user interface, application logic, database) to separate concerns and reduce complexity.

#### 6.**Architectural Complexity**

- **Complexity**: in a system architecture arises because of the number and the nature of the relationships between components in that system.
- **avoid** unnecessary software complexity:
	- **Localize relationships**: If there are relationships between components A and B, these are easier to understand if A and B are defined in the same module.
	- **Reduce shared dependencies**: Where components A and B depend on some other component or data, complexity increases.

- **Architectural Guidelines To Control Complexity**:

	![[Pasted image 20250113080134.png]](https://github.com/ali-bahr/Software-Engineering-Summaries/blob/main/images/Pasted%20image%2020250113080134.png)



#### **6. Cross-Cutting Concerns**

- **Definition**: Concerns that affect the entire system, such as **security**, **performance**, and **reliability**
- **Examples**: 
    - **Security**: Must be implemented across all layers.
        
    - **Performance**: Affects how components interact and communicate.
        
    - **Reliability**: Ensures the system continues to function despite failures.
- The existence of cross-cutting concerns is the reason why modifying a system after it has been designed to improve its security is often difficult.

#### **7. Distribution Architecture**

- **Client-Server Architecture**:
    
    - **Client**: Handles user interface and input.
        
    - **Server**: Manages business logic and data storage.
        
    - **Communication**: Typically uses HTTP, with data represented in XML or JSON.

	![[Pasted image 20250113081044.png]](https://github.com/ali-bahr/Software-Engineering-Summaries/blob/main/images/Pasted%20image%2020250113081044.png)        
- **Multi-Tier Architecture**:
    
    - **Web Server**: Handles client requests.
        
    - **Application Server**: Manages business logic.
        
    - **Database Server**: Stores and retrieves data.

		![[Pasted image 20250113081125.png]](https://github.com/ali-bahr/Software-Engineering-Summaries/blob/main/images/Pasted%20image%2020250113081125.png)

- **Service-Oriented Architecture (SOA)**:
    
    - **Stateless Services**: Components can be replicated and migrated across servers.
        
    - **Scalability**: Easier to scale as demand increases.
        
    - **Resilience**: More resilient to failure due to distributed nature.
	
		![[Pasted image 20250113081301.png]](https://github.com/ali-bahr/Software-Engineering-Summaries/blob/main/images/Pasted%20image%2020250113081301.png)
	

#### **8. Architectural Choices**

- **Database**:
    
    - **Relational (SQL)**: Suitable for structured data and transactions (e.g., e-commerce platforms).
        
    - **NoSQL**: Suitable for unstructured data and scalability (e.g., social media analytics, IoT systems).

- **Platform**:
    
    - **Web-Based**: Accessible via browsers.
        
    - **Mobile**: Requires separate front-end design due to device limitations (e.g., intermittent connectivity, power management).

- **Server**:
    
    - **In-House Servers**: Preferred by businesses concerned about cloud security.
        
    - **Cloud**: Suitable for consumer products with variable demand.

- **Open Source**:
    
    - **Advantages**: Reduces development costs and time-to-market.
        
    - **Disadvantages**: Limited control over evolution and potential licensing issues.

- **Development Tools**:
    
    - Influence architectural choices based on built-in assumptions (e.g., mobile development toolkits, web frameworks).




### **Question Bank**

1. **Which of the following are non-functional attributes of a software system?** (Select all that apply.)  
    A) Responsiveness.  
    B) Security.  
    C) Usability.  
    D) Maintainability.  
    
    **Correct Answers**: A, B, C, D
    
2. **Which of the following are true about reliability?** (Select all that apply.)  
    A) It ensures the system behaves as expected by users.  
    B) It is a non-functional attribute.  
    C) It is only relevant during the development phase.  
    D) It is unrelated to system performance.  
    
    **Correct Answers**: A, B
    

1. **Which of the following are true about the trade-off between maintainability and performance?** (Select all that apply.)  
    A) Monolithic architectures are easier to maintain but may suffer from performance issues.  
    B) Component-based architectures improve maintainability but may introduce performance overhead.  
    C) Performance is always more important than maintainability.  
    D) Maintainability is only relevant for small systems.  

	**Correct Answers**: A, B
    
2. **Which of the following are true about the trade-off between security and usability?** (Select all that apply.)  
    A) Layered security improves security but may reduce usability.  
    B) Too many security layers can frustrate users.  
    C) Security is always more important than usability.  
    D) Usability is only relevant for mobile applications.  
    
    **Correct Answers**: A, B
    

1. **Which of the following are true about component decomposition?** (Select all that apply.)  
    A) It involves breaking down large-scale components into finer-grained components.  
    B) It reduces system complexity.  
    C) It is only relevant for monolithic architectures.  
    D) It is unrelated to system performance.  

	**Correct Answers**: A, B
    
2. **Which of the following are true about layered architectures?** (Select all that apply.)  
    A) They separate concerns into different layers.  
    B) They reduce complexity by organizing components into layers.  
    C) They are only used in monolithic systems.  
    D) They are unrelated to system security.  
    
    **Correct Answers**: A, B
    
1. **Which of the following are true about client-server architecture?** (Select all that apply.)  
    A) The client handles the user interface.  
    B) The server manages business logic and data storage.  
    C) Communication typically uses HTTP.  
    D) It is only suitable for small systems.  
    
    **Correct Answers**: A, B, C
    
2. **Which of the following are true about service-oriented architecture (SOA)?** (Select all that apply.)  
    A) Services are stateless and can be replicated.  
    B) It is easier to scale as demand increases.  
    C) It is less resilient to failure than monolithic systems.  
    D) It is only suitable for mobile applications.  
    
    **Correct Answers**: A, B
    
1. **Which of the following are true about database choices?** (Select all that apply.)  
    A) Relational databases are suitable for structured data and transactions.  
    B) NoSQL databases are suitable for unstructured data and scalability.  
    C) SQL databases are always better than NoSQL databases.  
    D) NoSQL databases are only used for small systems.  
    
    **Correct Answers**: A, B
    
2. **Which of the following are true about cloud vs. in-house servers?** (Select all that apply.)  
    A) Cloud servers are suitable for consumer products with variable demand.  
    B) In-house servers are preferred by businesses concerned about cloud security.  
    C) Cloud servers are always more expensive than in-house servers.  
    D) In-house servers are only used for mobile applications.  
    
    **Correct Answers**: A, B









