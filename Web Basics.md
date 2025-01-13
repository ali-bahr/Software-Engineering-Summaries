#### **1. Web Basics**

- **IP Address**: A unique identifier for devices on a network, used to route data between them.
- **Domain Name**: A human-readable address (e.g., `facebook.com`) that translates to an IP address for network communication.
- **DNS (Domain Name System)**: Translates domain names (e.g., `facebook.com`) into IP addresses (e.g., `157.240.201.35`).
- **GeoDNS**: An extension of DNS that provides different IP addresses based on the client’s geographical location.
- **Port**: A numbered endpoint on a computer for network communication. Ports range from 0 to 65535 and allow multiple services to run simultaneously.

#### **2. HTTP & HTTPS**

- **HTTP (HyperText Transfer Protocol)**: A protocol for transferring and receiving information on the web. It operates as a request-response system.
    
    - **Features**:
        - Reliable (uses TCP/IP).
        - Divides messages into chunks for faster transmission.
        - Uses port 80.

- **HTTPS**: A secure version of HTTP that encrypts data using SSL/TLS.
    
    - **Features**:        
        - Uses port 443.
        - Requires a certificate (e.g., Let’s Encrypt for free certificates).

#### **3. CDN (Content Delivery Network)**

- A network of distributed servers that deliver web content (e.g., images, videos) efficiently by minimizing latency.

- **Benefits**:    
    - Improved performance.
    - Reduced latency.        
    - Bandwidth savings.
    - Increased availability.
    - Enhanced security (e.g., protection against DDoS attacks).


#### **5. Evolution of Websites**

- **Static Websites**: Serve HTML, CSS, and JavaScript files.
- **Dynamic Websites**: Use backend languages (e.g., PHP, NodeJS) to generate content dynamically.    
- **AJAX (Asynchronous JavaScript and XML)**: Allows partial page updates without refreshing the entire page.


#### **6. Deployment Basics**

- **Hosting Options**:
    
    - Shared hosting.
    - Virtual Private Servers (VPS).
    - Dedicated servers.
    - Cloud hosting (pay-as-you-go).

- **Deployment Steps**:
    
    - Choose a hosting provider.        
    - Set up DNS.
    - Access the server via SSH.
    - Install prerequisites (e.g., PHP, MySQL).
    - Upload project files (e.g., using FTP/SFTP).
    - Configure the server (e.g., environmental variables, Apache settings).
    - Generate and configure SSL certificates (e.g., using Certbot).
    - CI / CD

#### **7. File Transfer Protocols**

- **FTP (File Transfer Protocol)**:
    - Uses port 21.
    - Transfers data in plain text (less secure).

- **SFTP (Secure File Transfer Protocol)**:
    - Uses port 22.  
    - Encrypts data for secure transfers.
    - Supports key-based authentication.


#### **8. Web Development Concepts**

- **Cookies**: Small data stored on the client side, used for authentication, tracking, and session management.
- **Session Storage**: Stores data temporarily for a single browser session.
- **Local Storage**: Stores larger amounts of data persistently across sessions.
- **JWT (JSON Web Tokens)**: Used for authentication and authorization. Consists of a header, payload, and signature.

![[Pasted image 20250113033938.png]](https://github.com/ali-bahr/Software-Engineering-Summaries/blob/main/Pasted%20image%2020250113033938.png)

#### **9. OAuth**

- A protocol for authorization, allowing users to log in with third-party services (e.g., Facebook, Google).
    
- **Steps**:
    - User is redirected to the third-party login page.
    - User grants permission.
    - The application receives an access token.
    - The application uses the token to access user data.
- for ex:
	- The developer creates a facebook App and receives:
		1. Client id: can be used directly by user.
		2. Client Secret: is only used by the server.

	![[Pasted image 20250113034040.png]](https://github.com/ali-bahr/Software-Engineering-Summaries/blob/main/Pasted%20image%2020250113034040.png)


### **Question Bank for Lecture 2: Web Basics & Request Lifecycle**

1. **Which of the following are true about DNS?** (Select all that apply.)  
    A) It translates domain names into IP addresses.  
    B) It uses port 80 for communication.  
    C) GeoDNS provides different IP addresses based on the client’s location.  
    D) It is only used for static websites.  
    **Correct Answers**: A, C
    
2. **Which of the following are true about ports?** (Select all that apply.)  
    A) Ports range from 0 to 65535.  
    B) Port 80 is used for HTTPS.  
    C) Port 443 is used for HTTP.  
    D) Ports allow multiple services to run on the same IP address.  
    **Correct Answers**: A, D
    
1. **Which of the following are true about HTTP?** (Select all that apply.)  
    A) It uses port 80.  
    B) It encrypts data using SSL/TLS.  
    C) It divides messages into chunks for faster transmission.  
    D) It is a request-response protocol.  
    **Correct Answers**: A, C, D
    
2. **Which of the following are true about HTTPS?** (Select all that apply.)  
    A) It uses port 443.  
    B) It requires a certificate for encryption.  
    C) It is less secure than HTTP.  
    D) It is used for static websites only.  
    **Correct Answers**: A, B
    
1. **Which of the following are benefits of using a CDN?** (Select all that apply.)  
    A) Reduced latency.  
    B) Increased bandwidth costs.  
    C) Improved website performance.  
    D) Protection against DDoS attacks.  
    **Correct Answers**: A, C, D
    
2. **Which of the following are true about CDNs?** (Select all that apply.)  
    A) They cache content closer to users.  
    B) They increase the distance data has to travel.  
    C) They reduce bandwidth costs.  
    D) They are only used for static websites.  
    **Correct Answers**: A, C
    

1. **Which of the following are functions of a web server?** (Select all that apply.)  
    A) Serve static files (e.g., HTML, CSS).  
    B) Encrypt data using SSL/TLS.  
    C) Route requests to backend code.  
    D) Log and monitor activity.  
    **Correct Answers**: A, C, D
    
2. **Which of the following are examples of web servers?** (Select all that apply.)  
    A) Apache.  
    B) Nginx.  
    C) MySQL.  
    D) IIS.  
    **Correct Answers**: A, B, D
    
1. **Which of the following are true about deployment?** (Select all that apply.)  
    A) Shared hosting is the most expensive option.  
    B) Cloud hosting allows pay-as-you-go pricing.  
    C) SFTP is more secure than FTP.  
    D) DNS propagation is not required for deployment.  
    **Correct Answers**: B, C
    
2. **Which of the following are steps in deploying a web application?** (Select all that apply.)  
    A) Install prerequisites (e.g., PHP, MySQL).  
    B) Upload project files using FTP/SFTP.  
    C) Generate SSL certificates using Certbot.  
    D) Use port 21 for HTTPS.  
    **Correct Answers**: A, B, C
    

1. **Which of the following are true about cookies?** (Select all that apply.)  
    A) They are stored on the server side.  
    B) They are used for authentication and tracking.  
    C) They have a maximum size of 4KB.  
    D) They are transferred with every HTTP request.  
    **Correct Answers**: B, C, D
    
2. **Which of the following are true about JWT?** (Select all that apply.)  
    A) It consists of a header, payload, and signature.  
    B) It is used for authentication and authorization.  
    C) It is stored only on the server side.  
    D) It is encrypted using SSL/TLS.  
    **Correct Answers**: A, B
    

1. **Which of the following are true about OAuth?** (Select all that apply.)  
    A) It is used for user authentication with third-party services.  
    B) It requires a client ID and client secret.  
    C) It uses port 443 for communication.  
    D) It is only used for static websites.  
    **Correct Answers**: A, B
    
2. **Which of the following are steps in the OAuth process?** (Select all that apply.)  
    A) User is redirected to the third-party login page.  
    B) User grants permission to the application.  
    C) The application receives an access token.  
    D) The application uses the token to access user data.  
    **Correct Answers**: A, B, C, D
