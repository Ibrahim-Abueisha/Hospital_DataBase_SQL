# **Hospital_DataBase_SQL**
# DESCRIPTION OF THIS DATABASE

**The database represents an up running hospital and stores information about it’s operation like the following:**

  •	Stores information about the patient like his first name, last name, sex, diagnosis, email, phone number, age, and his Social Security number.
  
  •	For each employee it has his first name, last name, Social Security number, age, phone number, email, and sex.es slide. 
  
  •	For each Department there are its name, number, capacity, and the quantity of employees working in it. 
  
  •	Each medical specialization has its name, id and for how many years this is specialization exists in the hospital.
  
  •	We also have three particular employees have their own info and demonstrated like the following: 
  
   -	Doctors, having their last names, Social Security numbers, scientific degrees, field, years of experience.
  
   -	Nurses, having their last names, Social Security numbers, shift, and marital status. 
 
   -	Housekeepers, having their last names, Social Security numbers and working shifts.

  •	For each intensive care unit, there are its number, floor, and the landline phone number. Rooms also have this info in addition to the room capacity.
  
  •	Each operation can be performed has its name, unique id, ETA. The operation theater has its number and floor.
  
  •	Clinics have their names, unique ids, landline phone number and the floor.
  
  •	Finally, the database stores for each client his name, age, Email, phone number, social security number and whether he is visiting a patient or want to reserve a clinic appointment for an examination.


  
# Relationships and Business Rules

**All of these objects are connected to each other according to the following rules:**

  •	A doctor can manage only one specialization and each specialization is managed by only one doctor.
  
  •	Each doctor can supervise as many as possible from nurses, but each nurse is supervised by only one doctor.
  
  •	one doctor can examine multiple patients, but any patient can only be examined by one doctor. Each examination has a specific date, time, and period.
  
  •	Doctor can perform only one operation for a specific period, but the same operation can be performed by multiple doctors.
  
  •	Doctor can run only one clinic for a specific shift and the clinic can be run by only one doctor.
  
  •	A nurse can treat multiple patients, but the patient is treated by only one nurse.
  
  •	A nurse can participate in only one operation, but the operation can have multiple nurses participating in it.
  
  •	A nurse can take care of multiple rooms and intensive care units, but each intensive care unit and each room is taken care of by only one nurse. 
  
  •	A patient stays in only one room or an icu with an entry date and expected leaving date, but multiple patients can stay in the same room.
  
  •	A patient can have only one operation on a specific date and time and an operation can be performed on only one patient.
  
  •	An operation can take place in only one operation theater for a specific period.



# Relationships and Business Rules

**All of these objects are connected to each other according to the following rules:**

  •	A housekeeper handles many rooms and intensive care units, but each room and each intensive care unit can be handled by only one housekeeper.
  
  •	Each clinic belongs to only one specialization, but the same specialization can have multiple clinics belong to it.
  
  •	A client can visit multiple rooms and the same room can be visited by multiple clients. Each visit has a specific date and time.
  
  •	Also, a client can make appointments on certain dates and times to different clinics, multiple clients can make different appointments to same clinic. 
  
  •	Each Employee works in only one department with a certain salary, hiring date and working hours. The same department has many employees.
  
  •	Each employee can manage only one department and the department has only one manager. 


# NOTES

**TOTAL VS PARTIAL PARTICIPATION**

We have 13 total participations against 21 partial participations.


**RELATIONSHIPS ORDER**

We have 3 ternary relationships against 14 binary relationships.


**RELATIONSHIPS CARDINALITY**

We have:

-	6 one to one relationships,

-	12 one to many relationships,

-	2 many to many relationships. 
