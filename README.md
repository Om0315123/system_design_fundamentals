# system_design_fundamentals
As we are going to discuss the fundamentals of system design we will start with : 
## WHAT IS SYSTEM DESIGN ? 
 - Process of defining the architecture , components , modules , inteface and the data flow for a system to satisfy the needs of client or specify the requirements .
 - Always the Goal is to create well structured , efficient and well - organized to meet the the intended purpose.
## OBJECTIVES 
 - Practicality : System should targetting the intended audience.
 - Accuracy : Design should fullfill nearly all requirements.
 - Efficient
 - Reliability : Designing a system onto which the client can totally rely for the task it is intended too.
 - Scalabe : Should be adapatable to the future upgradation and changes.
## COMPONENTS 
 - A Load Balancer : It distributes the the tasks or traffic to multiple servers so that single server shouldn't get all the stress.
 - Key value store : Storage system that manage data as pairs of key and value ,it is often implemented  using distributed hash  table.
 - Blob Storage : service for storing large no of unstructured data . eg -  media files over youtube
 - Data Base : Organized collection of data and easy access modification.
 - Rate Limiter : Controls the max number of request a service can handle.
 - Monitoring Storage : Allows the administrative body to track and analyse infrastructure.
 - Distributed Messaging Queue : Felicitate Communication b/w the consumer and producer ensuring reliable message delivery
 - Distributed Unique ID Generator : Generates the unique id's for events and tasks in distributed  system.
 - Distributed Search : Allowss to search from the multiple sources.
 - Distributed Task Scheduler : Manage and allocate computational resources for executing tasks across a distributed system.
## Advantages of System Design 
- Reduces the Design Cost of a Product: By using established design patterns and reusable components, teams can lower the effort and expense associated with creating new software designs.
- Speedy Software Development Process: Using frameworks and libraries accelerates development by providing pre-built functionalities, allowing developers to focus on unique features.
- Saves Overall Time in SDLC: Streamlined processes and automation in the Software Development Life Cycle (SDLC) lead to quicker iterations and faster time-to-market.
- Increases Efficiency and Consistency of a Programmer: Familiar tools and methodologies enable programmers to work more effectively and produce uniform code, reducing the likelihood of errors.
- Saves Resources: Optimized workflows and shared resources minimize the need for redundant efforts, thereby conserving both human and material resources.
## System Design Life Cycle (SDLC) 
 - The System Design Life Cycle (SDLC) is a comprehensive process that outlines the steps involved in designing and developing a system, be it a software application, hardware solution, or an integrated system combining both.
 - The SDLC aims to ensure that the end product is reliable, scalable, and maintainable.
 - <img src='https://media.geeksforgeeks.org/wp-content/uploads/20241010133812082602/System-Design-Life-Cycle-22.jpg' length ='500' width ='550'>
## SYSTEM ARCHITECTURE
 - System architecture is a way in which we define how the components of a design are depicted design and deployment of software.
 - It is basically the skeleton design of a software system depicting components, abstraction levels, and other aspects of a software system.
 - System Architecture Patterns :
    - There are various ways to organize the components in software or system architecture. And the different predefined organization of components in software architectures are known as software architecture patterns.
 - Different types of System Architecture Patterns include :
    - Client-Server Architecture Pattern: Separates the system into two main components: clients that request services and servers that provide them.
    - Event-Driven Architecture Pattern: Uses events to trigger and communicate between decoupled components, enhancing responsiveness and scalability.
    - Microkernel Architecture Pattern: Centers around a core system (microkernel) with additional features and functionalities added as plugins or extensions.
    - Microservices Architecture Pattern: Breaks down applications into small, independent services that can be developed, deployed, and scaled independently.
# MODULARITY AND INTERFACE 
 - Modularity and interfaces in systems design are essential concepts that enhance flexibility and usability by breaking down complex systems into manageable components.
 - Modularity :
    - Modular design involves breaking down complex products into smaller, independent components or modules.
    - This allows each module to be developed and tested separately, making the overall system more flexible and easier to manage.
- Interface :
    - interfaces are the points where users interact with the system. This includes navigation elements, data input forms, and report displays.
# Evolution/Upgrade/Scaling of System 
 - Suppose there is a system with configurations of specific disk and RAM which was handling tasks. Now if we need to evolve our system or scale up, we have two options with us:
    - Vertical Scaling :
        - We are simply improving the processor by upgrading the RAM and disk size and many other components.
        - Note that here we are not caring about the scalability and availability of network bandwidth.
        - As per evolution we are working over the availability factor only considering scalability will be maintained. This is known as vertical scaling.
    - Horizontal Scaling :
        - In order to scale up, we need more systems (more chunks of blocks) and this is known as horizontal scaling.
    <img src='https://media.geeksforgeeks.org/wp-content/uploads/20221117172105/howtoevolveasystem.png' length='500' width='550'>
    
