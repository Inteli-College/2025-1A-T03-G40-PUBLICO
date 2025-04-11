# Public Report
This document aims to describe what was developed in the past ten weeks and how it contributed to the final project. This first of four modules was focused on understanding the problem from the user and company’s perspective and elaborating the general idea of the solution by mapping its main requisites and components. 

## I. Project Description
This project aims to help people identify which colors suit them best. It uses computer vision to analyze a person's appearance and determine the color palette, among twelve possibilities, that best suits them. A software tool will allow users to upload a photo of themselves and receive a color palette based on their appearance. Also, theoretical content about the process of personal color will help the user understand the importance of the tool. [1][2]

## II. Artifacts
In this module, the following artifacts were developed:
### 2.1 User Journey Map and Persona
These two artifacts were essential to understanding who the users were and how they would interact with the system. The user journey map shows the steps the user takes to achieve their goal, while the persona represents a fictional character that embodies the characteristics of the target audience. Two journey maps were created: one for the current process of personal color analysis and another for the future process with the software tool. This was important to identify the pain points and opportunities for improvement in the current process. [3][4]

### 2.2 Solution Description
This artifact describes the problem and the general idea of the solution. It also describes the benefits of the solution for the user and the company. The problem was described from both perspectives, which helped to understand the needs and expectations of both parties. The solution was described in a general way, without going into technical details, which allowed us to focus on the main idea and its benefits.

### 2.3 Value Proposition Canvas
This artifact was used to understand the value proposition of the solution. It describes how the solution meets the needs and expectations of the user and the company. The value proposition canvas was divided into two parts: the customer profile and the value proposition. The customer profile describes the jobs, pains, and gains of the target customer, while the value proposition outlines the products and services that address these needs and the pain relievers and gain creators that make the offering attractive to the customer. This is crucial to understand how the solution can create value for the user by addressing their needs and expectations. [5]

### 2.4 User Stories
The user stories were created to describe the main functionalities of the system. They were made following the INVEST model, which states that a good user story should be Independent, Negotiable, Valuable, Estimable, Small, and Testable. Each user story was measured by the size of the effort required to implement it and the priority of the feature. This helped to prioritize the development of the system and to focus on the most important functionalities for the user. [6]

### 2.5 Use Cases
Based on the user stories, use cases were created to describe the interactions between the user and the system. Each use case describes a specific scenario in which the user interacts with the system to achieve a goal. This helped to understand how the system should behave in different situations and to identify the main requirements for each functionality. The use cases were divided into normal flow and extensions, which helped to identify the main scenarios and the possible exceptions that could occur during the interaction. This is important to ensure that the system is robust and can handle different situations without failing. [7]

### 2.6 System Requirements
With the use cases in hand, the system requirements were created to describe the functional and non-functional requirements of the system. The functional requirements describe what the system should do, while the non-functional requirements describe how the system should behave. This helped to ensure that the system met the needs and expectations of the user and the company. [7]

### 2.7 Wireframe
A low-fidelity wireframe was created to represent the main screens of the system. The wireframe was created using Figma and was used to visualize the layout and structure of the main screens. This helped to understand how the user will interact with the system and to identify any potential usability issues. The wireframe was created based on the user journey map and the use cases, which helped to ensure that it meets the needs and expectations of the user. [8]

### 2.8 System Architecture
Here, we enter more in depth into the technical aspects of the system. The system architecture describes the main components of the system and how they interact with each other. It also describes the technology stack that will be used to implement the system. This is important to ensure that the system is scalable, reliable, and maintainable. Deployment and communication diagrams were created to show how each component will interact with each other. Also, a proof of concept was created to demonstrate the main functionality of uploading a photo and receiving a color palette. This helped to have a backbone structure of the system and understand in practice how the components will interact with each other. [9]

#### 2.8.1 Proof of Concept
A simple Next.js application was created with a form to upload a photo and a button to send it to the backend. The backend was implemented using NestJS, and it calls a FastAPI endpoint to perform the analysis. The FastAPI endpoint receives the image and returns a color palette in JSON format, which will be shown in the frontend. The convolutional model has not yet been implemented, but the proof of concept demonstrates the main flow and connection between the components. This helped to validate the architecture and the technology stack, as well as to identify any potential issues that could arise during the implementation.

## III. Conclusion
In conclusion, this first module focused on understanding the problem and planning the components of the solution. In the following three modules, the web application and the convolutional models will be developed and integrated to have a working MVP for the final project.

## IV. References
1. BROWN, J.; ROJAS, A. Determining Personal Colors Guide C-315. [s.l: s.n.]. Disponível em: <https://pubs.nmsu.edu/_c/C315.pdf >. 
2. XU, Pingyuan et al. Applications of artificial intelligence and machine learning in image processing. Frontiers in Materials, v. 11, p. 1431179, 2024.
3. GIBBONS, S. Journey Mapping 101. Disponível em: <https://www.nngroup.com/articles/journey-mapping-101 />.
4. HARLEY, A. Personas Make Users Memorable for Product Team Members. Disponível em: <https://www.nngroup.com/articles/persona />.
5. OSTERWALDER, Alexander et al. Value proposition design: How to create products and services customers want. John Wiley & Sons, 2015.
6. COHN, Mike. User stories applied: For agile software development. Addison-Wesley Professional, 2004.
7. STEPHENS, Matt; ROSENBERG, Doug. Use Case Driven Object Modeling with UML—Theory and Practice. Berkeley: Apress, 2007.
8. HAMM, M. J. Wireframing essentials: an introduction to user experience design: learn the fundamentals of designing the user experience for applications and websites. Birmingham: Packt Publishing, 2014.
9. FOWLER, Martin. UML essencial. 3. ed. Porto Alegre: Bookman, 2011. E-book. p.129. ISBN 9788560031382.
