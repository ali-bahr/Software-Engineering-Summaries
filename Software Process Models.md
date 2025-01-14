#### **1. Software Process Models**

- **Software Process**: A structured set of activities required to develop a software system. It involves:
    
    - **Specification**: Defining what the system should do.
    - **Design and Implementation**: Defining the system’s organization and implementing it.
    - **Validation**: Checking that the system meets customer requirements.
    - **Evolution**: Changing the system in response to changing customer needs.
- **Plan-Driven vs. Agile Processes**:
    
    - **Plan-Driven Processes**: All activities are ==planned in advance==, and progress is measured against the plan. Suitable for projects with stable requirements.
    - **Agile Processes**: ==Planning is incremental==, and the process is adaptable to changing requirements. Suitable for projects where requirements are likely to evolve.
#### **2. Waterfall Model**

- **Description**: A plan-driven model with distinct phases:
    
    1. **Requirements Definition**: Define what the system should do.
    2. **System and Software Design**: Design the system architecture and components.
    3. **Implementation and Unit Testing**: Write code and test individual units.
    4. **Integration and System Testing**: Integrate units and test the system as a whole.
    5. **Operation and Maintenance**: Deploy the system and maintain it over time.

	![[Pasted image 20250113044039.png]](https://github.com/ali-bahr/Software-Engineering-Summaries/blob/main/images/Pasted%20image%2020250113044039.png)

- **Advantages**:
    
    - Clear structure with distinct phases.        
    - Suitable for projects with well-understood and stable requirements.
    - Works well for large systems engineering projects with geographically dispersed teams.

- **Disadvantages**:
    
    - Inflexible to changing requirements.    
    - Not suitable for projects where requirements are likely to evolve.
    - Limited customer involvement during development.

#### **3. Incremental Development**

- **Description**: Specification, development, and validation are interleaved. The system is developed in increments, with each increment adding new functionality.
    
- **Advantages**:
    
    - Reduced cost of accommodating changing requirements.   
    - Easier to get customer feedback.
    - Rapid delivery of useful software to the customer.

- **Disadvantages**:
    
    - Process visibility is low, making it hard for managers to measure progress.        
    - System structure may degrade over time due to continuous changes.
    - Incorporating further changes becomes increasingly difficult and costly.

#### **4. Agile Software Engineering**

- **Core Principles**:
    
    - **Individuals and Interactions** over processes and tools.
    - **Working Software** over comprehensive documentation.
    - **Customer Collaboration** over contract negotiation.        
    - **Responding to Change** over following a plan.

- **Agile Methods**:
    
    - Focus on delivering functionality quickly.
    - Respond to changing product specifications.
    - Minimize development overheads.

- **Incremental Development in Agile**:
    
    - Development is done in increments, with each increment delivering a usable feature.
    - Features are prioritized, and the most important ones are implemented first.  
    - Users or surrogate users provide feedback after each increment.

	![[Pasted image 20250113045527.png]](https://github.com/ali-bahr/Software-Engineering-Summaries/blob/main/images/Pasted%20image%2020250113045527.png)

- **Agile development principles**:
    
    - **Involve the customer**
    - **Embrace change**: Expect the features of the product to change as we go. Adapt the software to cope with changes as they are made.
    - **Develop and deliver incrementally**         
    - **Maintain simplicity**: do what you can to eliminate complexity from the system.
    - **Focus on people, not things**: Trust the development team, Team members should be left to develop their own ways of working without being limited.




#### **5. Extreme Programming (XP)**

- **Description**: An agile method that emphasizes rapid, incremental development and delivery. It focuses on 12 key practices:

	1. **Incremental Planning**: Requirements are written as user stories, and priorities are set based on customer feedback.
	2. **Small Releases**: Minimal useful functionality is developed first, with frequent releases.
	3. **Test-Driven Development (TDD)**: Tests are written before code to clarify requirements and ensure code quality.
	4. **Continuous Integration**: Code is integrated into the system frequently, and all tests must pass before the new version is accepted.
	5. **Refactoring**: Code is continuously improved to maintain simplicity and readability.
	6. **Pair Programming**: Two developers work together on the same code to improve quality.
	7. **Collective Ownership**: All team members are responsible for the codebase.
	8. **On-Site Customer**: A customer representative is available to provide feedback and clarify requirements. 
	9. **Sustainable Pace**: Developers work at a sustainable pace to avoid burnout.
	10. **Simple Design**: The system is kept as simple as possible.
	11. **Metaphor**: A shared story or metaphor guides the development process.
	12. **Coding Standards**: Consistent coding standards are followed to maintain code quality.

The most widely used XP techniques (highlighted in red on the following pic):

![[Pasted image 20250113050234.png]](https://github.com/ali-bahr/Software-Engineering-Summaries/blob/main/images/Pasted%20image%2020250113050234.png)

#### **6. Choosing the Right Model**

- **Waterfall Model**: Suitable for projects with well-defined, stable requirements (e.g., large systems engineering projects).
- **Agile Model**: Suitable for projects where requirements are likely to change (e.g., mobile apps, startups).
- **Extreme Programming (XP)**: Suitable for projects requiring rapid development, frequent feedback, and high-quality code (e.g., web development, creative projects).



### **Question Bank**

1. **Which of the following are true about software processes?** (Select all that apply.)  
    A) They involve specification, design, implementation, validation, and evolution.  
    B) They are the same for all types of projects.  
    C) They can be plan-driven or agile.  
    D) They do not involve customer feedback.  
    **Correct Answers**: A, C
    
2. **Which of the following are characteristics of plan-driven processes?** (Select all that apply.)  
    A) All activities are planned in advance.  
    B) They are flexible to changing requirements.  
    C) Progress is measured against a plan.  
    D) They are suitable for projects with stable requirements.  
    **Correct Answers**: A, C, D
    

1. **Which of the following are phases of the waterfall model?** (Select all that apply.)  
    A) Requirements Definition.  
    B) System and Software Design.  
    C) Incremental Development.  
    D) Operation and Maintenance.  
    **Correct Answers**: A, B, D
    
2. **Which of the following are disadvantages of the waterfall model?** (Select all that apply.)  
    A) Inflexible to changing requirements.  
    B) Suitable for projects with evolving requirements.  
    C) Limited customer involvement during development.  
    D) Works well for large systems engineering projects.  
    **Correct Answers**: A, C
    
1. **Which of the following are advantages of incremental development?** (Select all that apply.)  
    A) Reduced cost of accommodating changing requirements.  
    B) Easier to get customer feedback.  
    C) Rapid delivery of useful software.  
    D) High process visibility for managers.  
    **Correct Answers**: A, B, C
    
2. **Which of the following are disadvantages of incremental development?** (Select all that apply.)  
    A) System structure may degrade over time.  
    B) Incorporating further changes becomes difficult.  
    C) High process visibility for managers.  
    D) Suitable for projects with stable requirements.  
    **Correct Answers**: A, B
    

1. **Which of the following are core principles of agile software engineering?** (Select all that apply.)  
    A) Individuals and interactions over processes and tools.  
    B) Comprehensive documentation over working software.  
    C) Customer collaboration over contract negotiation.  
    D) Following a plan over responding to change.  
    **Correct Answers**: A, C
    
2. **Which of the following are true about agile methods?** (Select all that apply.)  
    A) They focus on delivering functionality quickly.  
    B) They are suitable for projects with stable requirements.  
    C) They minimize development overheads.  
    D) They are inflexible to changing requirements.  
    **Correct Answers**: A, C
    

1. **Which of the following are widely adopted XP practices?** (Select all that apply.)  
    A) Test-Driven Development (TDD).  
    B) Continuous Integration.  
    C) Refactoring.  
    D) Comprehensive documentation.  
    **Correct Answers**: A, B, C
    
2. **Which of the following are true about Extreme Programming (XP)?** (Select all that apply.)  
    A) It emphasizes rapid, incremental development.  
    B) It requires detailed upfront planning.  
    C) It focuses on delivering high-quality code.  
    D) It is suitable for projects with stable requirements.  
    **Correct Answers**: A, C
     
1. **Which model is suitable for a project with well-defined, stable requirements?**  
    A) Waterfall.  
    B) Agile.  
    C) Extreme Programming (XP).  
    D) Incremental Development.  
    **Correct Answer**: A



