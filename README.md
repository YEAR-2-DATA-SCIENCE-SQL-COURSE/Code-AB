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

  ## Technical Approach 
  


  ## Database Design and Diagrams 

* ​Departments and Doctors Structure: The diagram shows how the departments table connects to the doctors table, while allowing doctors to manage other doctors using a manager ID field.  
* Appointments as a Link: The appointments table acts as a bridge connecting patients and doctors together to organize visits and track their statuses.  
* Prescriptions and Fast Search: It shows how appointments lead to prescriptions, which include a special search vector and GIN index for fast text searches.

<img width="1216" height="822" alt="WhatsApp Image 2026-11-07 at 4 56 26 PM" src="https://github.com/user-attachments/assets/aa042d56-763a-470b-acab-a0447947fe53" />



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
