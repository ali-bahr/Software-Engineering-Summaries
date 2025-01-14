#### **1. Introduction to Microservices**

- **Definition**: Microservices are small-scale, stateless, independent, and self-contained software components that perform a single responsibility. They communicate with each other over the internet using lightweight protocols.
- They are completely independent with their own database and UI management code.
- **Key Characteristics**:
    
    - **Self-contained**: Each microservice manages its own data and user interface.
        
    - **Lightweight**: Communication between microservices is efficient.
        
    - **Implementation-independent**: Microservices can be written in different programming languages and use different technologies.
        
    - **Independently deployable**: Each microservice runs in its own process and can be deployed independently.
        
    - **Business-oriented**: Microservices are designed to implement specific business capabilities.


#### **3. Cohesion and Coupling**

- **Cohesion**: A measure of how closely related the parts of a component are. High cohesion means all parts of a microservice work together to achieve a single responsibility.
    
- **Coupling**: A measure of how dependent one microservice is on others. Low coupling means microservices are independent and can be changed without affecting others.

#### **4. API Gateway**

- **Purpose**: Acts as a single entry point for all client requests to microservices.
- **Functions**:
    
    - **Rate Limiting**: Controls the number of requests a client can make.
    - **Error Handling**: Manages errors and retries failed requests.
    - **Caching**: Stores responses to reduce load on microservices.
- **Implementation**:
    
    - **Reverse Proxy**: Using tools like Nginx.
    - **Custom API Gateway**: Built using frameworks like Node.js.


#### **5. Microservices Communication**

- **Synchronous Communication**:
    
    - The client waits for a response from the server.
    - Example: RESTful APIs.
        
- **Asynchronous Communication**:
    
    - The client does not wait for a response and continues processing.
    - Example: Message brokers like Kafka, RabbitMQ.
        
- **Direct vs. Indirect Communication**:
    
    - **Direct**: Microservices communicate directly with each other.
    - **Indirect**: Microservices communicate through a message broker.

#### **6. Data Design in Microservices**

- **Data Isolation**: 
	- Each microservice should manage its own data with minimal sharing.
	- If data sharing is unavoidable, you should design microservices so that most sharing is ‘read-only’.
- **Eventual Consistency**: Databases used by different replicas microservices may not be consistent at all times but they must eventually become consistent.
- **Pending Transaction Log**: Used to track changes and ensure eventual consistency across microservices.

#### **7. Orchestration vs. Choreography**

- **Orchestration**:
    
    - A central service (orchestrator) coordinates the workflow between microservices.
        
    - Easier to manage but can become a single point of failure.
        
        ![[Pasted image 20250114013800.png]](https://github.com/ali-bahr/Software-Engineering-Summaries/blob/main/images/Pasted%20image%2020250114013800.png)
- **Choreography**:
    
    - Microservices communicate directly with each other without a central coordinator.
        
    - More flexible but harder to debug and test.
	      
	    ![[Pasted image 20250114013831.png]](https://github.com/ali-bahr/Software-Engineering-Summaries/blob/main/images/Pasted%20image%2020250114013831.png)


#### **8. Failure Handling**


- **Timeouts**: A mechanism to detect unresponsive services by setting a maximum wait time for a response.
    
- **Circuit Breaker**: Prevents further requests to a failed service until it recovers, avoiding system slowdowns.

#### **10. Deployment**

- **Continuous Deployment**: Automatically deploying new versions of microservices as soon as changes are made and tested.
    
- **Versioned Services**: Maintaining multiple versions of a microservice to allow rollback in case of issues.
  
  ![[Pasted image 20250114014902.png]](https://github.com/ali-bahr/Software-Engineering-Summaries/blob/main/images/Pasted%20image%2020250114014902.png)
  
  
  
  
### **Question Bank**
1. **Which of the following are characteristics of microservices?** (Select all that apply.)  
    A) Self-contained.  
    B) Lightweight communication.  
    C) Tightly coupled.  
    D) Independently deployable.  
    
    **Correct Answers**: A, B, D
    
2. **Which of the following are true about monolithic architecture?** (Select all that apply.)  
    A) All components are tightly coupled.  
    B) Easier to scale than microservices.  
	C) Difficult to maintain as the system grows.  
    D) Components are deployed independently.  
    
    **Correct Answers**: A, C
    
1. **Which of the following are true about cohesion?** (Select all that apply.)  
    A) High cohesion means all parts of a microservice work together to achieve a single responsibility.  
    B) Low cohesion means microservices are independent.  
    C) High cohesion reduces the complexity of a microservice.  
    D) Low cohesion is preferred in microservices architecture.  
    
    **Correct Answers**: A, C
    
1. **Which of the following are true about coupling?** (Select all that apply.)  
    A) Low coupling means microservices are independent.  
    B) High coupling means microservices are tightly dependent on each other.  
    C) Low coupling makes it easier to change microservices without affecting others.  
    D) High coupling is preferred in microservices architecture.  
    
    **Correct Answers**: A, B, C
    
1. **Which of the following are functions of an API Gateway?** (Select all that apply.)  
    A) Rate limiting.  
    B) Error handling.  
    C) Caching.  
    D) Direct communication between microservices.  
    
    **Correct Answers**: A, B, C
    
2. **Which of the following are true about API Gateway implementation?** (Select all that apply.)  
    A) It can be implemented using a reverse proxy like Nginx.  
    B) It can be customized using frameworks like Node.js.  
    C) It is only used for synchronous communication.  
    D) It is not necessary in microservices architecture.  
    
    **Correct Answers**: A, B
    
1. **Which of the following are true about synchronous communication?** (Select all that apply.)  
    A) The client waits for a response from the server.  
    B) It is typically used in RESTful APIs.  
    C) It is faster than asynchronous communication.  
    D) It is not suitable for microservices architecture.  
    
    **Correct Answers**: A, B
    
2. **Which of the following are true about asynchronous communication?** (Select all that apply.)  
    A) The client does not wait for a response.  
    B) It is typically used with message brokers like Kafka.  
    C) It is slower than synchronous communication.  
    D) It is not suitable for microservices architecture.  
    
    **Correct Answers**: A, B
    
1. **Which of the following are true about data design in microservices?** (Select all that apply.)  
    A) Each microservice should manage its own data.  
    B) Data sharing between microservices should be minimized.  
    C) Eventual consistency is acceptable in microservices architecture.  
    D) ACID transactions are always used in microservices.  
    
    **Correct Answers**: A, B, C
    
2. **Which of the following are true about eventual consistency?** (Select all that apply.)  
    A) It ensures that databases will eventually become consistent.  
    B) It is implemented using a pending transaction log.  
    C) It is not suitable for microservices architecture.  
    D) It requires immediate consistency across all microservices.  
    
    **Correct Answers**: A, B
    
1. **Which of the following are true about timeouts?** (Select all that apply.)  
    A) They are used to detect unresponsive services.  
    B) They can slow down the system if a service fails.  
    C) They are not necessary in microservices architecture.  
    D) They are replaced by circuit breakers in all cases.  
    
    **Correct Answers**: A, B
    
2. **Which of the following are true about circuit breakers?** (Select all that apply.)  
    A) They prevent further requests to a failed service.  
    B) They are used to detect unresponsive services.  
    C) They are slower than timeouts.  
    D) They are not necessary in microservices architecture.  
    **Correct Answers**: A, B
    
1. **Which of the following are true about RESTful services?** (Select all that apply.)  
    A) They are stateless.  
    B) They use HTTP verbs like GET, POST, PUT, and DELETE.  
    C) They are not suitable for microservices architecture.  
    D) They typically use JSON or XML for data representation.  

	**Correct Answers**: A, B, D
    
2. **Which of the following are true about RESTful service operations?** (Select all that apply.)  
    A) GET is used to read a resource.  
    B) POST is used to create a resource.  
    C) PUT is used to update a resource.  
    D) DELETE is used to remove a resource.  
    
    **Correct Answers**: A, B, C, D

1. **Which of the following are true about continuous deployment?** (Select all that apply.)  
    A) It automates the deployment of new versions of microservices.  
    B) It relies on automated testing to ensure quality.  
    C) It is not suitable for microservices architecture.  
    D) It requires manual intervention for every deployment.  
    **Correct Answers**: A, B
    
2. **Which of the following are true about versioned services?** (Select all that apply.)  
    A) They allow rollback to previous versions in case of issues.  
    B) They are not necessary in microservices architecture.  
    C) They complicate the deployment process.  
    D) They are only used in monolithic systems.  
    **Correct Answers**: A