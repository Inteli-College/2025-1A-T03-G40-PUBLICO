# Public Report
This document outlines the work completed over the past ten weeks as part of the second module of the project. The focus of this phase was the development of the main Web Application, encompassing both frontend and backend services. This is the second of four modules that collectively contribute to the final project deliverable.

## I. Project Description
The project aims to assist users in identifying the colors that suit them best. Leveraging computer vision techniques, the system analyzes a user's appearance and suggests one of twelve predefined color palettes tailored to their features. Users can upload a photo and receive a personalized palette. Additionally, the application includes educational content to help users understand the theory behind personal color analysis and the value of the tool. [1][2]

## II. Artifacts
### 2.1 Domain Model
A domain model was developed to define the core entities and their relationships within the application. A domain model is a visual representation of a specific area of knowledge or business, using key concepts, vocabulary, and relationships to understand the real-world objects and their interactions within that area. It's a way to model the relevant parts of a business or problem domain, focusing on the data and rules within that domain. [3]

### 2.2 Wireframe
A high-fidelity wireframe was designed using Figma to depict the application's main screens. It includes branding elements such as colors and logos, and is based on prior artifacts including low-fidelity wireframes, the user journey map, and use cases. This visual prototype helped identify potential usability issues early and guided the implementation of the user interface. [4]

### 2.3 Backend
The backend was implemented using NestJS, a scalable and modular server-side framework built with TypeScript. It handles requests from the frontend, processes uploaded images, and returns the appropriate color palette. Additionally, it interfaces with FastAPI, which will be used to run the convolutional model (to be developed in upcoming modules).

#### 2.3.1 Unit Tests
Unit tests were implemented using Jest to validate core business logic in the backend. These tests ensure individual components function correctly in isolation, allowing for early detection and resolution of bugs. [5]

### 2.4 Frontend
The frontend was developed using Next.js, a React-based framework that supports server-side rendering. It handles the user interface, enabling users to upload photos and receive results from the backend. The codebase uses TypeScript for type safety and maintainability.

### 2.4.1 Unit Tests
Unit tests were written using Jest and React Testing Library to verify utility functions and component rendering. These tests ensure the frontend behaves as expected across various scenarios.

### 2.4.2 End-to-End Tests
End-to-end (E2E) tests were developed using Cypress to simulate real user flows, such as registration, login, photo upload, and color palette retrieval. These tests validate that all components work seamlessly together. 

End-to-end (E2E) testing is a software testing method that verifies the complete workflow of an application from start to finish, simulating real-world user scenarios. It ensures that all integrated components of the system function correctly together, from the user interface to the database and external services. [6]

### 2.5 Integration
The integration between the frontend and backend was achieved through RESTful APIs. E2E tests were updated to verify the integration and ensure a smooth and functional user experience across the full application stack.

### 2.6 Deployment
#### 2.6.1 Deployment Documentation
The application was deployed using Render, a cloud hosting platform that supports continuous deployment from Git repositories. Render provides essential infrastructure features such as automatic TLS, CDN, autoscaling, and DDoS protection. The deployment includes:

- Backend Services: ColorAnalysisService and VisionPalette
- Frontend Service: PersonalColorApp

Additionally, the PostgreSQL database is hosted on Aiven, which offers automated backups, high availability, and strong security (encryption in transit and at rest). [7][8]

#### 2.6.2 Cost Analysis
A cost analysis was conducted for hosting the application on AWS in a production environment. It includes estimated expenses for:
- EC2 instance for frontend and backend services
- RDS instance for the PostgreSQL database

### 2.7 Final Presentation
A final presentation was prepared to showcase to the company the completed module, including a live demonstration of the application. The presentation highlighted the key features, architecture,  cost analysis, and a discussion about data collection for the convolutional model, providing an overview of the work accomplished in this module.

## III. Conclusion
This module successfully delivered a functional and integrated Web Application, laying the groundwork for the final system. The frontend and backend components are now in place, allowing for seamless user interaction and image handling. In the upcoming modules, the convolutional models will be developed and integrated, leading to a fully functional MVP for the final project.

## IV. References
1. BROWN, J.; ROJAS, A. Determining Personal Colors Guide C-315. [s.l: s.n.]. Disponível em: <https://pubs.nmsu.edu/_c/C315.pdf >. 
2. XU, Pingyuan et al. Applications of artificial intelligence and machine learning in image processing. Frontiers in Materials, v. 11, p. 1431179, 2024.
3. EVANS, Eric. **Domain-driven design: tackling complexity in the heart of software.** Addison-Wesley Professional, 2004.
4. HAMM, M. J. **Wireframing essentials: an introduction to user experience design: learn the fundamentals of designing the user experience for applications and websites.** Birmingham: Packt Publishing, 2014.
5. CLIFTON, M. **Unit Testing Succinctly**. [s.l: s.n.]. p. 1-128
6. **The Complete Guide to End-to-End Testing.** [s.l: s.n.]. Disponível em: <https://spring2019.stpcon.com/wp-content/uploads/2018/12/SB_EBK_End-to-End-Testing.pdf>.
7. **Getting Started with Render.** Disponível em: <https://app-generator.dev/docs/deployment/render/index.html>. Acesso em: 24 jun. 2025.
8. **Set up hosted PostgreSQL® database for FREE.** Disponível em: <https://aiven.io/free-postgresql-database>. Acesso em: 24 jun. 2025.
