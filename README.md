 Code-AB

## Project Title
Kigali Hospital Patients Records 

## Group Members
| Member Name | Role |
| :-- | :-- | 
| Mussab Altoom | Leader |
| Muhammed Abdalkareem | Member |
| Adel Salah | Member | 
| Ahmed Elmotez | Member |
| Muhammed Ahmed | Member |
| Ahmed Ibrahim | Member |
| Abdalla Abulgasim | Member |
| Hassan | Member |

## Introduction 
This is A Relational Database Management System for managing Patients Records, Dates and Departments in Kigali Hospital. 

## Problem Statements
The purpose for creating A Database is solve some problems in storing data manually, The common problems that solve is like data redundancy, lack of explicit relationship constraints,  we can not rely on paper  for storing can cause data loss, physical damage, it is very hard to share data across multiple hospitals, it is very hard to access fast data.

## Objectives 
* Design an organized Database.
* Enable easily to share the data across multi hospitals.
* It is very easy to make analysis in the data.
* Manipulate in the data very easy delete, update just through queries.

## Research and Key Concepts
* Using RDBMS for organizing data (PostgreSQL) related tables.
* Create Tables with the right Constraints.
* Connect the tables  together using primary and foreign key to be relational RDBMS.
* Insert data into the tables following the constraints for patients,doctors...
* Execute queries for fast and easy access data retrieval.
* Apply join to show the relation between the tables e.g one_to_one.

## 7. Technical Approach

This section detail the technical design, architectural patterns, software tools, and engineering methodologies employed to design, normalize, and deploy the relational database system.

### 7.1 Architectural Overview & System Patterns
The system is built upon a **Layered Client-Server Relational Architecture**, emphasizing modular design, scalability, and robust data consistency:
* **Relational Database Tier:** Utilizes an RDBMS engine (MySQL / PostgreSQL) to enforce structural schema constraints, ensure strict ACID compliance, and manage indexed relational mappings[span_0](start_span)[span_0](end_span).
* **Data Processing & Automation Tier:** Implements modular SQL scripts for Data Definition (DDL), Data Manipulation (DML), and advanced programmatic structures including Database Views, Triggers, and Stored Procedures.
* **Structured Repository Organization:** Maintains a strict separation of concerns across dedicated project directories[span_1](start_span)[span_1](end_span):
  * `sql/`: Contains fully documented, modular DDL and DML execution scripts[span_2](start_span)[span_2](end_span).
  * `diagrams/`: Houses visual modeling artifacts, including conceptual and logical Entity-Relationship Diagrams (ERDs)[span_3](start_span)[span_3](end_span).
  * `sample-data/`: Stores curated datasets used for query execution, validation, and benchmarking[span_4](start_span)[span_4](end_span).

### 7.2 Technology Stack
* **Database Management System (DBMS):** MySQL / PostgreSQL managed via phpMyAdmin, pgAdmin, or Visual Studio Code integrated tooling.
* **Version Control & Collaboration:** Git & GitHub for granular history tracking and collaborative repository management.
* **Data Modeling & Specification:** Markdown for documentation; industry-standard visual tools (MySQL Workbench / draw.io) for schema modeling.

### 7.3 Core Engineering Methodologies
1. **Requirements Elicitation & Conceptual Schema Design:**
   - Identified domain-specific business entities, core attributes, and system-wide operation rules.
   - Formulated conceptual ER diagrams establishing explicit entity relationships, participation constraints, and cardinalities (1:1, 1:N, M:N)[span_5](start_span)[span_5](end_span).
2. **Logical Schema Transformation & Relational Normalization:**
   - Mapped conceptual entities directly into logical tables with defined Primary Keys (PK) and Foreign Keys (FK).
   - Applied **Third Normal Form (3NF) Normalization** guidelines to systematically eliminate data redundancy and prevent operational anomalies (Insertion, Update, and Deletion).
3. **Physical Implementation & Declarative Scripting:**
   - Authored DDL scripts incorporating strict data type definitions, `NOT NULL` constraints, `UNIQUE` indexes, and referential integrity cascades (`ON DELETE`, `ON UPDATE`).
   - Populated the schema via DML scripts and constructed relational queries involving complex multi-table `JOIN` operations, aggregate functions, and grouped metrics.
4. **Validation, Integrity Verification & Performance Testing:**
   - Conducted rigorous edge-case testing to ensure foreign key integrity and constraint enforcement under non-standard inputs.
   - Verified that query execution outputs directly fulfill the domain objectives outlined in the project scope.
  
  


  ## Database Design and Diagrams 

* ​Departments and Doctors Structure: The diagram shows how the departments table connects to the doctors table, while allowing doctors to manage other doctors using a manager ID field.  
* Appointments as a Link: The appointments table acts as a bridge connecting patients and doctors together to organize visits and track their statuses.  
* Prescriptions and Fast Search: It shows how appointments lead to prescriptions, which include a special search vector and GIN index for fast text searches.

<img width="1216" height="822" alt="WhatsApp Image 2026-11-07 at 4 56 26 PM" src="https://github.com/user-attachments/assets/aa042d56-763a-470b-acab-a0447947fe53" />

## 

## Real World Applications
This system can be used in Kigali hospitals for :
* **Patient Registration:** Fast intake at reception to avoid long lines.
* **Medical Records:** Safe and quick access to patient medical history.
* **Appointments:** Easy scheduling for doctors, rooms, and clinic visits.
* **Hospital Reports:** Clear data to help management track visits and resources.

  ## Challenges and Recommendations

  ## Challenges
  * **Data Safety:** Protecting sensitive patient records from Unauthorized access.
  * **Staff Adaptation:** Helping hospital staff move smoothly from paper to a digital system.
  * **performance:** Keeping the system fast as patient data grow.
 
    ## Recommendations
    * **Role Access :** Give each staff member access only to the data they need.
    * **Staff Training:** Provide clear training to make the transition easy for doctor and nurses.
    * **System Maintenance :** Run regular backups and optimize the database for for high speed.


## Future Improvements
* implement an online patient portal where patients can view their medical records, appointment, and prescriptions.
add an appointment booking and scheduling system to reduce waiting times.
* integrate the system with laboratory and pharmacy departments for seamless sharing of test results and prescriptions. 
* enable SMS or email reminders for appointments and medication schedules. 
* enhance security by adding two-factor authentication and stronger data encryption.
* develop a mobile application for doctors, nurses, and patients to access records conveniently.

## References 
