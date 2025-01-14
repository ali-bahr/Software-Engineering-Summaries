
#### **1. Software Quality**

- **Definition**: Software quality refers to the attributes that make a software product reliable, secure, usable, and maintainable.
    
- **Key Quality Attributes**:
    
    - **Reliability**: The software performs its intended functions without failure.
        
    - **Availability**: The software is accessible when needed.
        
    - **Security**: The software protects against unauthorized access and data breaches.
        
    - **Resilience**: The software can recover from failures and continue to operate.
        
    - **Usability**: The software is easy to learn and use.
        
    - **Maintainability**: The software is easy to modify and update.
        
    - **Responsiveness**: The software responds quickly to user inputs.
      
      
#### **2. Programming for Reliability**

- **Fault Avoidance**: Writing code in a way that minimizes the introduction of faults.
    
- **Input Validation**: Ensuring that user inputs conform to expected formats and values.
    
- **Failure Management**: Implementing mechanisms to handle failures gracefully and minimize their impact on users.

#### **3. Refactoring**

- **Definition**: Refactoring is the process of improving the internal structure of code without changing its external behavior.
    
- **Goals**:
    
    - **Reduce Complexity**: Make the code easier to read, understand, and modify.
        
    - **Improve Maintainability**: Make future changes easier and less error-prone.
        
- **Code Smells**: Indicators of potential problems in the code, such as:
    
    - **Large Classes**: Violate the single responsibility principle.
        
    - **Long Methods**: Indicate that a method is doing too much.
        
    - **Duplicated Code**: Increases the risk of inconsistencies.
        
    - **Meaningless Names**: Make the code harder to understand.
        
    - **Unused Code**: Adds unnecessary complexity.

#### **4. Input Validation**

- **Purpose**: Ensures that user inputs are in the correct format and within acceptable ranges.
    
- **Methods**:
    
    - **Built-in Validation Functions**: Use functions provided by frameworks (e.g., email validation).
        
    - **Explicit Comparisons**: Compare inputs against allowed values or lists.
        
    - **Regular Expressions**: Define patterns that inputs must match.


#### **5. Failure Management**

- **Auto-Save**: Automatically save user data at regular intervals to minimize data loss in case of failure.
    
- **Activity Logging**: Keep a log of user actions to allow recovery of work in case of failure.
    
- **External Service Failure**: Handle failures in external services by checking return codes and validating results.


#### **6. Software Diagrams**

- **Sequence Diagram**: Shows the interaction between objects in a system over time.
    
- **UML Class Diagram**: Represents the structure of a system by showing classes, attributes, methods, and relationships.
    
- **Use Case Diagram**: Illustrates the interactions between users (actors) and the system.





### **Question Bank**

1. **Which of the following are key quality attributes of software?** (Select all that apply.)  
    A) Reliability.  
    B) Security.  
    C) Usability.  
    D) Maintainability.  

	**Correct Answers**: A, B, C, D
    
2. **Which of the following are true about software quality?** (Select all that apply.)  
    A) Reliability ensures the software performs its intended functions without failure.  
    B) Usability ensures the software is easy to learn and use.  
    C) Maintainability ensures the software is easy to modify and update.  
    D) Security is not important for software quality.  
    
    **Correct Answers**: A, B, C
    
1. **Which of the following are techniques for improving software reliability?** (Select all that apply.)  
    A) Fault avoidance.  
    B) Input validation.  
    C) Failure management.  
    D) Ignoring user inputs.  

	**Correct Answers**: A, B, C
    
2. **Which of the following are true about fault avoidance?** (Select all that apply.)  
    A) It involves writing code in a way that minimizes the introduction of faults.  
    B) It is not important for reliable programming.  
    C) It reduces the likelihood of errors in the code.  
    D) It is only relevant for large systems.  
    
    **Correct Answers**: A, C
    
1. **Which of the following are true about refactoring?** (Select all that apply.)  
    A) It improves the internal structure of code without changing its external behavior.  
    B) It reduces code complexity.  
    C) It makes the code harder to maintain.  
    D) It is only necessary for large systems.  
    
    **Correct Answers**: A, B
    
2. **Which of the following are examples of code smells?** (Select all that apply.)  
    A) Large classes.  
    B) Long methods.  
    C) Duplicated code.  
    D) Meaningful variable names.  
    
    **Correct Answers**: A, B, C
    
1. **Which of the following are methods of implementing input validation?** (Select all that apply.)  
    A) Built-in validation functions.  
    B) Explicit comparisons.  
    C) Regular expressions.  
    D) Ignoring user inputs.  
    
    **Correct Answers**: A, B, C
    
2. **Which of the following are true about input validation?** (Select all that apply.)  
    A) It ensures that user inputs are in the correct format.  
    B) It is not important for security.  
    C) It prevents database pollution.  
    D) It is only necessary for web applications.  
    
    **Correct Answers**: A, C
    
1. **Which of the following are true about failure management?** (Select all that apply.)  
    A) Auto-save minimizes data loss in case of failure.  
    B) Activity logging allows recovery of user actions in case of failure.  
    C) External service failures should be ignored.  
    D) Failure management is not important for reliable programming.  
    
    **Correct Answers**: A, B
    
2. **Which of the following are true about external service failures?** (Select all that apply.)  
    A) They should be handled by checking return codes.  
    B) They are not important for reliable programming.  
    C) The results of external service calls should be validated.  
    D) External services are always reliable.  
    
    **Correct Answers**: A, C
    
1. **Which of the following are true about UML class diagrams?** (Select all that apply.)  
    A) They show the structure of a system by representing classes, attributes, and methods.  
    B) They are not useful for understanding system behavior.  
    C) They can show relationships like inheritance and association.  
    D) They are only used for small systems.  

	**Correct Answers**: A, C
    
2. **Which of the following are true about sequence diagrams?** (Select all that apply.)  
    A) They show the interaction between objects over time.  
    B) They are not useful for understanding system behavior.  
    C) They can represent synchronous and asynchronous communication.  
    D) They are only used for large systems.  
    
    **Correct Answers**: A, C
    
