#### **2. GraphQL**

- **Definition**: A query language for APIs developed by Facebook, allowing clients to request exactly the data they need.
    
- **Key Features**:
    
    - **Flexible Querying**: Clients can specify the exact fields they need, reducing over-fetching and under-fetching.
        
    - **Strongly Typed Schema**: The schema evolves without breaking existing queries.
        
    - **Single Endpoint**: Unlike REST, which uses multiple endpoints, GraphQL uses a single endpoint for all queries.
        
- **Use Cases**: Applications requiring flexible data retrieval, such as social media platforms (e.g., Facebook, GitHub).
  
  
  
#### **3. gRPC**

- **Definition**: A high-performance RPC (Remote Procedure Call) framework developed by Google, using **Protocol Buffers (protobuf)** for efficient binary serialization.
    
- **Key Features**:
    
    - **High Performance**: Low CPU and bandwidth usage due to binary serialization.
        
    - **Platform Independent**: Works across different programming languages.
        
    - **Real-time Communication**: Supports bidirectional streaming.
        
- **Use Cases**: Microservices, high-performance systems, and real-time communication (e.g., Google APIs).
  
  
#### **4. SOAP (Simple Object Access Protocol)**

- **Definition**: A protocol for exchanging structured information in web services using XML.
    
- **Key Features**:
    
    - **Standardization**: Built-in standards for security and ACID transactions.
    - **Enterprise-Level**: Often used in legacy systems and enterprise integrations.        
    - **Verbosity**: Uses XML, which can be more verbose compared to JSON.
        
- **Use Cases**: Enterprise-level integrations, financial systems, and legacy applications.
  
  


#### **5. WebSocket**

- **Definition**: A protocol for real-time, bidirectional communication between clients and servers.
    
- **Key Features**:
    
    - **Real-time Communication**: Enables low-latency, bidirectional messaging.
        
    - **Stateful**: Maintains an open connection between client and server.
        
    - **Use Cases**: Chat applications, gaming, stock trading platforms, and real-time updates.
        



#### **Comparison of Protocols**

| Feature             | gRPC                       | GraphQL                 | SOAP               | REST API            | WebSocket             |
| ------------------- | -------------------------- | ----------------------- | ------------------ | ------------------- | --------------------- |
| **Payload Format**  | Protobuf                   | JSON                    | XML                | JSON/XML            | Binary/Text           |
| **Protocol**        | HTTP/2                     | HTTP                    | HTTP               | HTTP                | WebSocket             |
| **Flexibility**     | Somewhat                   | Yes                     | No                 | Somewhat            | Yes                   |
| **Real-time**       | Yes                        | No                      | No                 | No                  | Yes                   |
| **Schema**          | Yes                        | Yes                     | No                 | No                  | No                    |
| **Standardization** | Yes                        | No                      | Yes                | Somewhat            | No                    |
| **Use Cases**       | Microservices, Google APIs | Flexible data retrieval | Enterprise systems | Web and mobile APIs | Real-time chat, Games |


### **Question Bank (MCQs)**

#### **1. REST API**

1. **Which HTTP method is used to create a resource in REST API?**
    
    - A) GET
        
    - B) POST
        
    - C) PUT
        
    - D) DELETE
        
    - **Answer**: B) POST
        
2. **Which of the following are principles of RESTful services? (Select all that apply)**
    
    - A) Stateless
        
    - B) URI Addressable
        
    - C) Use of XML or JSON
        
    - D) Stateful
        
    - **Answer**: A, B, C
        
3. **What is the primary data format used in REST APIs?**
    
    - A) XML
        
    - B) JSON
        
    - C) Protobuf
        
    - D) Binary
        
    - **Answer**: B) JSON
        

---

#### **2. GraphQL**

1. **What is the main advantage of GraphQL over REST API?**
    
    - A) It uses XML for data representation.
        
    - B) It allows clients to request only the data they need.
        
    - C) It is stateful.
        
    - D) It uses multiple endpoints.
        
    - **Answer**: B) It allows clients to request only the data they need.
        
2. **Which of the following is true about GraphQL? (Select all that apply)**
    
    - A) It uses a single endpoint for all queries.
        
    - B) It is strongly typed.
        
    - C) It is primarily used for real-time communication.
        
    - D) It reduces over-fetching and under-fetching of data.
        
    - **Answer**: A, B, D
        
3. **Which company developed GraphQL?**
    
    - A) Google
        
    - B) Facebook
        
    - C) Microsoft
        
    - D) Amazon
        
    - **Answer**: B) Facebook
        

---

#### **3. gRPC**

1. **Which of the following is true about gRPC? (Select all that apply)**
    
    - A) It uses Protocol Buffers for serialization.
        
    - B) It is platform-independent.
        
    - C) It is primarily used for real-time communication.
        
    - D) It uses HTTP/2 as the underlying protocol.
        
    - **Answer**: A, B, D
        
2. **What is the primary advantage of using gRPC?**
    
    - A) It uses JSON for data representation.
        
    - B) It is highly performant due to binary serialization.
        
    - C) It is stateful.
        
    - D) It is primarily used for legacy systems.
        
    - **Answer**: B) It is highly performant due to binary serialization.
        
3. **Which of the following is a use case for gRPC?**
    
    - A) Real-time chat applications
        
    - B) Enterprise-level integrations
        
    - C) High-performance microservices
        
    - D) Flexible data retrieval
        
    - **Answer**: C) High-performance microservices
        

---

#### **4. SOAP**

1. **Which of the following is true about SOAP? (Select all that apply)**
    
    - A) It uses XML for data representation.
        
    - B) It is primarily used for real-time communication.
        
    - C) It is highly standardized.
        
    - D) It is often used in enterprise-level integrations.
        
    - **Answer**: A, C, D
        
2. **What is the primary disadvantage of SOAP?**
    
    - A) It is not standardized.
        
    - B) It is verbose due to the use of XML.
        
    - C) It is not suitable for enterprise systems.
        
    - D) It does not support ACID transactions.
        
    - **Answer**: B) It is verbose due to the use of XML.
        
3. **Which transport protocols can SOAP use? (Select all that apply)**
    
    - A) HTTP
        
    - B) SMTP
        
    - C) WebSocket
        
    - D) FTP
        
    - **Answer**: A, B
        

---

#### **5. WebSocket**

1. **Which of the following is true about WebSocket? (Select all that apply)**
    
    - A) It enables real-time, bidirectional communication.
        
    - B) It is stateless.
        
    - C) It is widely used in chat applications.
        
    - D) It uses HTTP/2 as the underlying protocol.
        
    - **Answer**: A, C
        
2. **What is the primary advantage of WebSocket over REST API?**
    
    - A) It uses JSON for data representation.
        
    - B) It enables real-time communication.
        
    - C) It is highly standardized.
        
    - D) It is primarily used for legacy systems.
        
    - **Answer**: B) It enables real-time communication.
        
3. **Which of the following is a use case for WebSocket?**
    
    - A) Enterprise-level integrations
        
    - B) Real-time stock trading platforms
        
    - C) Flexible data retrieval
        
    - D) High-performance microservices
        
    - **Answer**: B) Real-time stock trading platforms
        

---

#### **Comparison Questions**

1. **Which protocol is best suited for real-time communication?**
    
    - A) REST API
        
    - B) GraphQL
        
    - C) gRPC
        
    - D) WebSocket
        
    - **Answer**: D) WebSocket
        
2. **Which protocol is best suited for high-performance microservices?**
    
    - A) REST API
        
    - B) GraphQL
        
    - C) gRPC
        
    - D) SOAP
        
    - **Answer**: C) gRPC
        
3. **Which protocol is best suited for flexible data retrieval?**
    
    - A) REST API
        
    - B) GraphQL
        
    - C) gRPC
        
    - D) SOAP
        
    - **Answer**: B) GraphQL
        
4. **Which protocol is best suited for enterprise-level integrations?**
    
    - A) REST API
        
    - B) GraphQL
        
    - C) gRPC
        
    - D) SOAP
        
    - **Answer**: D) SOAP
        
5. **Which protocol is best suited for real-time traffic management in a Smart City platform?**
    
    - A) REST API
        
    - B) GraphQL
        
    - C) gRPC
        
    - D) WebSocket
        
    - **Answer**: D) WebSocket

