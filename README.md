# Orphanage Database Management System

A Microsoft Access-based relational database management system designed to organize, manage, and monitor information related to an orphanage.

The system manages various types of information, including children's biodata, health and education history, donors, donations, expenses, events, orphanage administrators, and other administrative data.

---

## Overview

Managing information in an orphanage requires organized and accessible data related to children, administration, donations, financial activities, and events.

This project develops a relational database system using **Microsoft Access** to simplify data management and improve accessibility of information.

The database integrates multiple entities and relationships into a structured system that allows users to retrieve information through tables, queries, forms, and reports.

The final system provides several information outputs, including:

- Children's Biodata
- Children's History
- Donations / Receipts
- Expenses
- Foundation Administrators
- Events

---

## Objectives

The main objectives of this project are:

- To design a structured relational database for an orphanage.
- To organize information related to children and orphanage operations.
- To establish relationships between related data entities.
- To simplify data retrieval through database queries.
- To provide a user-friendly interface through Microsoft Access forms.
- To generate structured reports for operational and administrative purposes.
- To support more efficient monitoring and management of orphanage information.

---

## System Scope

The database covers several operational areas of the orphanage, including:

- Children's personal information
- Parents or guardians
- Children's education
- Children's health records
- Donors
- Donations and receipts
- Operational expenses
- Events
- Event committees
- Event participants
- Foundation administrators
- Administrative positions

---

## Database Design

The database was designed using a relational database approach.

The design process consists of several stages:

1. System Analysis
2. Conceptual Data Model
3. Logical Data Model
4. Physical Database Design
5. Database Implementation

---

## System Analysis

The system analysis stage focused on identifying the information and operational processes required by the orphanage.

The analysis considered:

- Children's information management
- New child admission
- Donation management
- Financial management
- Event management
- Administrative information
- Education records
- Health records
- User interaction
- Data accessibility

The analysis served as the basis for designing the database structure and relationships.

---

## Conceptual Data Model

The conceptual design describes the main entities and relationships within the orphanage information system.

The database conceptual model consists of the following main entities:

- Education
- Health
- Child
- Event
- Foundation Administrator
- Position
- Parent / Guardian
- Expense
- Donation / Receipt
- Donor

The relationships between these entities represent how information is connected within the orphanage's operational processes.

---

## Logical Data Model

The logical database design converts the conceptual model into a relational database structure.

The logical design defines:

- Tables
- Primary keys
- Foreign keys
- Relationships between tables
- Data organization

The database tables are connected through foreign keys to maintain relationships and support data integrity.

---

## Database Implementation

The database was implemented using **Microsoft Access**.

The implementation includes:

- Tables
- Queries
- Forms
- GUI
- Reports

These components work together to provide a structured interface for managing and retrieving orphanage information.

---

# Database Tables

The database contains several tables representing different entities and operational activities.

## Event Table

The Event table stores information about events organized by the orphanage.

The table contains information such as:

- Event ID
- Event name
- Event location
- Event date

---

## Child Table

The Child table stores detailed information about children living in the orphanage.

The information includes:

- Child ID
- Gender
- First name
- Last name
- Photo
- Age
- Date of birth
- Admission date
- Departure date
- Parent / guardian ID

---

## Donor Table

The Donor table stores information about individuals or organizations that provide donations to the orphanage.

The information includes:

- Donor ID
- Donation date
- Donation method
- Donor identification information

---

## Position Table

The Position table stores the administrative positions available within the orphanage or foundation.

The table includes:

- Position ID
- Position type

---

## Last Education Level Table

The Last Education Level table stores information about the latest educational level associated with a child.

The table includes:

- Education level ID
- Child ID

---

## Health Table

The Health table stores health examination information for children.

The information includes:

- Health record ID
- Examination date
- Diagnosis
- Child ID

---

## Parent / Guardian Table

The Parent / Guardian table stores information about the parents or guardians associated with children.

The information includes:

- Parent / guardian ID
- Full name
- Gender
- Address

---

## Event Committee Table

The Event Committee table records administrators or staff members involved in organizing events.

The table connects:

- Administrator ID
- Event ID

---

## Education Table

The Education table stores information about educational institutions associated with children.

The information includes:

- Education ID
- School name
- Admission year
- Graduation year
- Education level
- Child ID

---

## Donation / Receipt Table

The Donation / Receipt table records donations received by the orphanage.

Donations can include monetary and non-monetary contributions.

The table contains information such as:

- Receipt ID
- Amount of money
- Item name
- Donor ID
- Administrator ID

---

## Expense Table

The Expense table records operational expenses of the orphanage.

The information includes:

- Expense ID
- Expense date
- Amount
- Event ID
- Administrator ID

---

## Foundation Administrator Table

The Foundation Administrator table stores information about individuals involved in managing the foundation or orphanage.

The table includes:

- Administrator ID
- Full name
- Gender
- Position ID

---

## Event Participant Table

The Event Participant table records children participating in events organized by the orphanage.

The table connects:

- Child ID
- Event ID

---

# Database Queries

Queries were developed to simplify information retrieval from the database.

The implemented queries include:

## Event Query

The Event Query retrieves event information, including:

- Event ID
- Location
- Date
- Event name

---

## Children's Biodata Query

The Children's Biodata Query allows users to retrieve children's personal information.

The information includes:

- Child ID
- Gender
- First name
- Last name
- Photo
- Age
- Date of birth
- Admission date
- Departure date

---

## Donation / Receipt Query

The Donation / Receipt Query provides a summary of donations received from donors.

The information includes:

- Donor ID
- Date
- Donation method
- Donor name
- Amount
- Item name
- Administrator ID
- Administrator name

---

## Expense Query

The Expense Query provides a summary of orphanage expenses.

The information includes:

- Event name
- Expense date
- Expense amount
- Administrator ID

---

## Children's History Query

The Children's History Query summarizes information related to children's history.

The information includes:

- Child ID
- First name
- Gender
- Diagnosis
- Education level

---

## Position Query

The Position Query provides information about foundation administrators and their positions.

The information includes:

- Position ID
- First name
- Gender
- Position type

---

# User Interface

Microsoft Access Forms were used to provide a graphical interface for users.

A total of **8 forms** were developed:

- 6 forms used as references for reports
- 2 forms used as application interfaces for users

The GUI provides users with access to several information areas without requiring them to directly interact with database tables.

---

# GUI Features

The main GUI provides access to:

- Children's Biodata
- Donations / Receipts
- Expenses
- Events
- Positions
- Children's History

Users can select the required information and retrieve related records through the interface.

---

## Children's Biodata

Users can search for a child by entering the child's first name.

The system then retrieves information such as:

- Child ID
- Gender
- First name
- Age
- Date of birth
- Admission date
- Departure date

---

## Donations / Receipts

Users can enter a donor's name to retrieve related donation information.

The system displays information such as:

- Donor ID
- Date
- Donation method
- Donor name
- Amount
- Item name

---

## Expenses

Users can enter an event name to retrieve related expense information.

The system displays:

- Expense date
- Expense amount

---

## Events

Users can search for an event by entering its name.

The system retrieves:

- Event ID
- Location
- Date
- Event name

---

## Foundation Positions

Users can search for an administrator position to retrieve related information.

The system displays:

- Position ID
- Gender
- Position type

---

## Children's History

Users can enter a child's first name to retrieve information related to the child's history.

The system displays:

- Child ID
- Gender
- Diagnosis
- Latest education level

---

# Reports

Reports were created to present database information in a structured and readable format.

The main reports cover:

- Children's Biodata
- Children's History
- Donations / Receipts
- Expenses
- Foundation Administrators
- Events

Reports allow the information retrieved from the database to be presented in a more organized format for administrative purposes.

---

# Results

The implemented database successfully integrates information related to children and orphanage operations into a relational database system.

The system provides users with access to:

- Children's biodata
- Children's health information
- Children's education information
- Parent / guardian information
- Donor information
- Donation records
- Expense records
- Event information
- Event participants
- Foundation administrators
- Administrative positions

The GUI allows users to retrieve information through search-based forms, while queries and reports provide structured access to the resulting information.

---

# Key Findings

### 1. Relational database design organizes interconnected information

The project demonstrates how different types of orphanage information can be organized into related entities and tables.

### 2. Queries simplify information retrieval

Database queries allow users to retrieve specific information without manually searching through individual tables.

### 3. Forms improve user interaction

Microsoft Access forms provide a more accessible interface for users who do not need to directly interact with database tables.

### 4. Reports improve information presentation

Reports organize retrieved database information into structured outputs that can be used for administrative purposes.

### 5. Database integration supports operational monitoring

Integrating children's information, donations, expenses, events, and administrative data into a single database provides a more centralized approach to information management.

---

# Limitations

Several limitations should be considered for this project:

- The database was developed using Microsoft Access, which may not be suitable for large-scale multi-user deployments.
- The project focuses primarily on data management and retrieval rather than advanced analytics.
- The database interface is designed for the specific operational requirements defined during the project.
- Data security and user access control could be further developed for deployment in a real-world environment.
- The current system does not provide web-based or mobile access.
- The database would require additional testing and validation before being deployed in an actual orphanage environment.

---

# Future Improvements

Potential improvements include:

- Implementing role-based user access.
- Adding stronger data validation.
- Improving database security and backup procedures.
- Developing a web-based database interface.
- Developing a mobile-friendly interface.
- Adding automated dashboards and data visualization.
- Integrating the database with other information systems.
- Adding more advanced reporting and analytics capabilities.
- Implementing automated backup and recovery mechanisms.

---

# Tools & Technologies

- Microsoft Access
- Relational Database Management System (RDBMS)
- Entity Relationship Modeling
- Conceptual Data Model (CDM)
- Physical Data Model (PDM)
- Database Queries
- Database Forms
- Database Reports

---

