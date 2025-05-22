# Assignments from SQL Database Design & Programming (CTS2433) 2023  
This course is designed to familiarize students with SQL (Structured Query Language) in a relational database environment to include database programming and development. A series of database application assignments using SQL commands is designed to promote competency in ER (Entity Relationship) database modeling, database creation, database programming, and database optimization. The objective is to build a working knowledge and hands-on understanding of SQL.  
### Rest of assignments are uploaded in each folder, with more complex more SQL queries and concepts
 
# Module 2
### Determine the functional dependencies that exist in the following table and then convert this table to an equivalent collection of tables that are in third normal form.  
```
OFFICE_NUM -> OFFICE_NAME
ADDRESS -> SQR-FT, BDRMS, FLOORS, MONTHLY_RENT, OWNER_NUM
OFFICE (OFFICE_NUM, OFFICE_NAME)
PROPERTY (ADDRESS, SQR_FT, BDRMS, FLOORS, MONTHLY_RENT, OWNER_NUM))
```
### Determine the functional dependencies that exist in the following table and then convert this table to an equivalent collection of tables that are in third normal form.
```
PROPERTY_ID -> OFFICE_NUM, ADDRESS
ADDRESS -> SQR_FT, BDRMS, FLOORS, MONTHLY_RENT, OWNER_NUM
OWNER_NUM -> LAST_NAME, FIRST_NAME
PROPERTY (PROPERTY_ID, OFFICE_NUM, ADDRESS)
LOCATION (ADDRESS, SQR_FT, BDRMS, FLOORS, MONTHLY_RENT, OWNER_NUM)
OWNER (OWNER_NUM, LAST_NAME, FIRST_NAME)
```
### StayWell also rents out properties on a weekly basis to students attending summer school in the Seattle area. Design a database to meet the following requirements, using the shorthand representation and a diagram of your choice.
For each student renter, list his or her number, first name, middle initial, last name, address, city, state, postal code, telephone number, and e-mail address.
```
STUDENT (STUDENT_NO, FIRST_NAME, MIDDLE_INITIAL, LAST_NAME, ADDRESS, CITY, STATE, POSTAL_CODE, TELEPHONE_NO, EMAIL)
```
For each property, list the office number, property address, city, state, postal code, square footage, number of bedrooms, number of floors, maximum number of persons that can sleep in the unit, and the base weekly rate.
```
PROPERTY (OFFICE_NO, ADDRESS, CITY, STATE, POSTAL_CODE, SQR_FT, BDRMS, FLOORS, MAX_PERSONS, WEEKLY_RATE)
```
For each rental agreement, list the renter number, first name, middle initial, last name, address, city, state, postal code, telephone number, start date of the rental, end date of the rental, and the weekly rental amount. The rental period is one or more weeks.  
```
RENTAL (RENTER_NO, FIRST_NAME, MIDDLE_INITIAL, LAST_NAME, ADDRESS, CITY, STATE, POSTAL_CODE, TELEPHONE_NO, START_DATE, END_DATE, WEEKLY_RENTAL)
```

# Module 3

### 1. Create a table named SUMMER_SCHOOL_RENTALS. The table has the same structure as the PROPERTY table shown in Figure 3-48 except the PROPERTY_ID and OFFICE_NUMBER columns should use the NUMBER data type and the MONTHLY_RENT column should be changed to WEEKLY_RENT. Execute the command to describe the layout and characteristics of the SUMMER_SCHOOL_RENTALS table.
![mod3q1](https://github.com/user-attachments/assets/0c58646d-26ae-4bc6-9497-607bf49ff71a)

![mod3q1b](https://github.com/user-attachments/assets/34d38cd9-bd3d-4ad3-be1a-28ebf25da0ec)

### 2.	Add the following row to the SUMMER_SCHOOL_RENTALS table: property ID: 13; office ID: 1; address: 5867 Goodwin Ave; square feet: 1,650; bedrooms: 2; floors 1; weekly rent: 400; owner number: CO103.
![mod3q2](https://github.com/user-attachments/assets/96099dcc-0456-441b-aed7-858674df0f3a)

### 3.	Delete the SUMMER_SCHOOL_RENTALS table.
![mod3q3](https://github.com/user-attachments/assets/38ba2731-916b-4d12-bc5a-ede44cefda03)

### 4.	Run the script file for the StayWell database to create the six tables and add records to the tables. Be sure to select the script file for the particular DBMS that you are using (MySQL, Oracle, or SQL Server). (Note: If you do not have the script files for this text, ask your instructor for assistance.)
-	I believe I did this correctly, I’m not sure what to put for this question but I clicked SQL scripts in oracle and uploaded the file with Oracle at the end of the name.

### 5.	Confirm that you have created the tables correctly by describing each table and comparing the results to Figures 3-48.
![mod3q5](https://github.com/user-attachments/assets/9cd4d7f5-4827-4f7a-be30-3a67a2c99647)

![mod3q5b](https://github.com/user-attachments/assets/1ab44bc3-2b87-43f9-80d8-42ae5c86bfe3)

![mod3q5c](https://github.com/user-attachments/assets/9c9d91fa-0add-470c-9de3-838ad5b4771f)

![mod3q5d](https://github.com/user-attachments/assets/69c68d37-2456-44f0-aa2f-701ed990bde8)

![mod3q5e](https://github.com/user-attachments/assets/3651d584-4963-4547-90ad-3ad44fb6efbb)

![mod3q5f](https://github.com/user-attachments/assets/cd2f74d1-a115-4ede-8abc-6417cd85a845)


### 6.	Confirm that you have added all data correctly by viewing the data in each table and comparing the results to Figures 1-4, 1-5, 1-6, 1-7, 1-8 and 1-9 in Module 1.  
Below are screenshots showing I have all the correct data, residents I copied from excel because it was taking multiple screenshots.  Also, I had issues with the script for oracle when it came to adding the dates in the SERVICE_REQUESTS table so I had to add each row manually, after reformatting the dates.  Then the table wasn’t ordered by SERVICE_ID even though I had it set as the primary key, so I ran a query that ordered it by SERVICE_ID for the screenshot below.

![mod3q6](https://github.com/user-attachments/assets/9df175bb-8863-4142-a554-6905ee60213e)

![mod3q6b](https://github.com/user-attachments/assets/a0e6b209-e0f8-483f-b32d-6a346b2e8c98)

![mod3q6c](https://github.com/user-attachments/assets/19a65d25-6910-4d4e-bc0b-d0e7f1a4d422)

![mod3q6d](https://github.com/user-attachments/assets/41ad8b3c-56c7-435c-952e-5ad8cb857d94)

![mod3q6e](https://github.com/user-attachments/assets/75d53c8a-4764-4246-92cf-8f2484c9a147)
