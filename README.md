# Pharmacy-Database
Created a relational database for a pharmacy using **Python Jupyter Notebook** that allows efficient storage, retrieval, and manipulation of data related to patients, prescriptions, and medications.

## Logic of Database 
## Relations
[x] Patient: Stores information about patients, such as their unique identifier(patient_id: Primary key), first name, last name, patient number, and their insurances’ information.

[x] Prescriptions: Stores information about prescriptions issued to patients. It includes attributes such as prescription ID (Primary Key), patient ID (foreign key referencing the Patient relation), medication ID (foreign key referencing the Medications relation), dosage, prescribed date and name of prescribing doctor.

[x] Medications: Stores information about the medications available at the pharmacy. It includes attributes like medication ID (Primary key), medicine name, medicine’s unit price, medicine’s expiration date.

## Constraints
[x] Primary Keys: Each relation should have a primary key that uniquely identifies each record. For example, Patient ID in the Patient relation, Prescription ID in the Prescriptions relation, and Medication ID in the Medications relation are the Primary Keys for our Pharmacy database.

[x] Foreign Keys: Appropriate foreign keys should be used to establish relationships between the tables. For example, the patient ID in the Prescriptions relation references the Patient ID in the Patient relation, and the medication ID in the Prescriptions relation references the Medication ID in the Medications relation.

[x] Other constraints: Additional constraints such as data types, nullability, unique constraints, etc. are also added as per the specific requirements of the pharmacy application.

## List of Modules

## Helper Functions

[x]def SelectQ: Takes a table name, an identifier column, and a value, and selects the row where the identifier column equals the value from the table. Returns the selected row.

[x] def DeleteQ: Takes a table name, an identifier column, and a value, and deletes the row where the identifier column equals the value from the table.

[x] def InsertQ: Takes a table name and a list of values to insert into the table. Inserts the values into the table and returns the row ID of the newly inserted row.

[x] def UpdateQ: Takes a table name, a column name, a new value, an identifier column name, and an old value. Updates the row in the table where the identifier column equals the old value with the new value.

[x] def executeQ: Takes a SQL query and executes and prints the result.

## Tables

The database includes three tables: Medications, Patients, and Prescriptions.

[x] Medications table has columns for med_id, med_name, unit_price, and expiration_date.

[x] Patients table has columns for patient_id, patient_fname, patient_lname, phone_number, and insurance.

[x] The Prescriptions table has columns for prescription_id, med_id, patient_id, dosage, date_prescribed, and prescribing_doctor. It also has foreign key constraints that reference the med_id and patient_id columns in the Medications and Patients tables, respectively.


## ER Diagram

![alt text](https://github.com/Myesha-Mahazabeen/Pharmacy-Database/blob/main/ER_Diagram.png)
 
