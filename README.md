Project Title: Hospital Management System Deployment on GCP Cloud Platform with Compliance to HIPAA

Name: Nicole Udochukwu

Start Date: 2nd June 2024

End Date: 21st August 2024

Role: Cloud Security Engineer

Project Overview

As the GCP Cloud Security Engineer, I spearheaded the development of an innovative hospital management system that adheres to HIPAA compliance. This project implemented a robust three-tier architecture on the Google Cloud Platform (GCP), ensuring security, scalability, and reliability in managing sensitive healthcare data.

Architecture

![Hipaa-GCP drawio AB](https://github.com/user-attachments/assets/9983fd9f-d0b8-4651-ad5b-aa0dec5cf654)

The system was designed with a three-tier architecture, consisting of:

*  Frontend: Built using Node.js and React.js, delivering a responsive and user-friendly interface.

*  Backend: Developed in Java using JDK 17 and Maven, ensuring a high-performance server-side application.

*  Database: Utilized Google Cloud SQL (MySQL) for a managed and secure relational database solution.
  

Security and Compliance

To ensure HIPAA compliance, I implemented comprehensive security measures throughout the development lifecycle, including:

1. SonarCloud code analysis for identifying vulnerabilities.

2. Conducted rigorous code reviews and security audits to uphold the highest security standards.

3. Implemented Google Cloud IAM for secure user authentication and authorization.

4. Developed firewall rules for inbound and outbound traffic control via Google Cloud Firewall.

   
Tools and Technologies Used

*  Git/GitHub: Utilized as a version control system to clone and manage the codebase for both backend and frontend applications.
*  Draw.io: Employed to create a visual representation of the three-tier architecture, illustrating the interactions between frontend, backend, and database components.
*  Confluence: Leveraged as a knowledge management platform to store, share, and collaborate on project documentation.
*  Jira: Used to plan, track, and manage the development and deployment of the hospital management system, ensuring efficient project execution.
*  Slack: Facilitated team communication, enabling quick discussions, information sharing, and feedback exchange among team members.
*  Google Cloud IAM: Provides identity and access management capabilities, ensuring secure authentication and authorization for users accessing the servers.
*  Google Cloud Firewall: Controls inbound and outbound network traffic, protecting servers from unauthorized access and threats by enforcing specified security rules and 
   policies.
*  Google Compute Engine: Provided a scalable and secure environment for hosting the application, allowing for the deployment of multiple virtual machines to support 
   different workloads and applications.
*  Google Cloud DNS: Enabled the creation of DNS records, routing traffic to the application and allowing users to access it via a custom domain name.
*  Google Cloud VPC: Established a secure and isolated network environment for the application, segregating it from the public internet.
*  Public and Private IP: Assigned public and private IP addresses to each server (backend, frontend, and database), facilitating secure access and communication.
*  Port Configuration: Configured ports to enable communication between servers and applications, ensuring seamless data exchange.

Frontend Development Tools
*  Node.js: Served as the JavaScript runtime environment for building and running the frontend application.
*  React.js: Used as the JavaScript library for building reusable UI components and managing the application's state.
*  JavaScript, HTML, CSS: Used for client-side scripting, structuring, and styling web pages.
*  NPM: Node Package Manager (NPM) was used to manage dependencies and install required packages for the project.

Backend Development Tools
* Java: Used as the primary programming language for backend development.
* JDK 17: Provided the Java Development Kit for compiling and running Java applications.
* Maven: Managed dependencies and automated the build process for the Java-based backend application.

Database Management
* Google Cloud SQL (MySQL): Used as the managed relational database service for storing and managing data.
* Cloud SQL Studio: Utilized for managing database connections and operations efficiently.

Infrastructure Setup

1 Resource Organization: Created a GCP project and set up organizational units for managing related resources.

2 Virtual Private Cloud (VPC): Created a VPC with subnets for segregating traffic and enhancing security.

<img width="916" alt="hipaa 22" src="https://github.com/user-attachments/assets/e6f1f629-0b95-4622-843a-af3712229507">

3 Firewall Rules: Configured Google Cloud firewall rules for managing access based on defined policies.

<img width="941" alt="hipaa 21" src="https://github.com/user-attachments/assets/98fef5ee-0d43-4dd3-a4cf-b950ba3449bb">

4 Compute Engine Instances: Provisioned Compute Engine instances for frontend, backend, and database tiers, ensuring encryption using SSL/TLS.

Database Creation and Server Configuration

== Cloud SQL Configuration:

* Created a Cloud SQL instance and configured MySQL with high availability.
* Set up the instance to enforce SSL connections for secure communication.

== Remote Connection Configuration:
* Configured the Cloud SQL instance to allow connections from specific IP addresses for enhanced security.

== Peering Connection:
* Established a private VPC peering connection between the backend Compute Engine instance and the Cloud SQL database to ensure secure and low-latency communication.

<img width="947" alt="700" src="https://github.com/user-attachments/assets/0e1e5001-3a03-4ee7-abdd-247042d7d8ea">


== Validation and Testing:
* Tested the setup using Cloud SQL studio to ensure the database connection was operationally efficient.
  
<img width="960" alt="hipaa 7" src="https://github.com/user-attachments/assets/de037a54-ad9a-4c82-875a-8681bad188ed">

== Security Measures:
* Enable Cloud SQL IAM roles for fine-grained access control.
* Implemented best practices for database user management and access.


Backend Creation and Configuration
== Firewall Configuration:
* Set up firewall rules allowing TCP traffic on relevant ports;
  8080 for backend communication
  22 for configuration
  frontend subnet

== Server Access:
* Used SSH via Google Cloud Console for server management.

== Setup Steps:
* Updated the VM and installed JDK 17, Maven, and MySQL Client.

<img width="960" alt="hipaa 3" src="https://github.com/user-attachments/assets/8a1531f0-7077-4e69-82d7-0ef6945d0293">

* Cloned the backend code from GitHub and configured for deployment.
* Applied Cross-Origin Resource Sharing (CORS) security to restrict access to the frontend domain.

<img width="960" alt="Sunday-hipaa" src="https://github.com/user-attachments/assets/e9b68395-b866-42d0-8fb2-4d62542afbc8">


==Application Deployment:
* Packaged and executed the application using Maven.
  
<img width="869" alt="hipaa 6" src="https://github.com/user-attachments/assets/46afaf0e-c40d-4e9c-a81c-4ceb8bce2adf">

<img width="931" alt="hipaa 13" src="https://github.com/user-attachments/assets/0307b29a-284e-44b4-b6a1-82f400dd0bec">

<img width="933" alt="706" src="https://github.com/user-attachments/assets/83b0f484-b0db-4926-8a19-32775663803d">

== Security Measures:
* Closed unnecessary ports and restricted access to the backend server.

Frontend Creation and Server Configuration

== Firewall Configuration:
* Set up firewall rules allowing TCP traffic on relevant ports;
  443 for public access
  22 for configuration
  3000 for application to run 

== Server Access:
* Used SSH via Google Cloud Console for server management.

== Setup Steps:
* Updated the VM to ensure it had the latest security patches and updates.
* Installed Node.js, which is required for the frontend application.
* Installed npm (Node Package Manager) to manage dependencies and install project-specific libraries.
* Cloned the frontend code from GitHub, ensuring the latest version of the code is used.
* Configured the frontend to bind with the backend server on port 8080, allowing communication between the two services.
* Installed project-specific dependencies using npm, ensuring all required libraries are available.
* Started the development server to test and develop the application locally.
  
<img width="960" alt="705" src="https://github.com/user-attachments/assets/1732e7f6-7d7c-4afa-9851-901129bd3c9d">


==Application Testing and Deployment:
* Verified the application was functioning as expected and running on port 3000.
  
<img width="909" alt="701" src="https://github.com/user-attachments/assets/cd394931-69b7-4a08-8b92-6624d239059a">

<img width="945" alt="703" src="https://github.com/user-attachments/assets/ae1db9c6-8b17-4726-9a8c-fe8d9eadfa02">


== Security Measures:
* Closed unnecessary ports.

DNS Configuration with Namecheap
* Domain Purchase: Purchased a domain from Namecheap for the hospital management system.
  
DNS Settings:
* Logged into the Namecheap account and navigated to the Domain List.
* Selected the purchased domain and clicked on "Manage."
* Under the "Advanced DNS" tab, added the following records:
* A Record: Pointed to the public IP address of the frontend Compute Engine instance.
* CNAME Record: Configured for subdomains as needed (e.g., www).
* Propagation Check: Used online tools to check DNS propagation and ensure the domain was resolving correctly to the application.






