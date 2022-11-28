
## Working with Default and Check 
```bash

CREATE SCHEMA College;
CREATE TABLE students
(
	id INT NOT NULL PRIMARY KEY,
    Name VARCHAR(20) NOT NULL,
    age INT NOT NULL CHECK(age >= 18),
    gender VARCHAR(10) NOT NULL ,
    phone VARCHAR(10) NOT NULL UNIQUE,
    city VARCHAR(20) NOT NULL DEFAULT 'AGRA'
);

INSERT INTO students VALUES
(
	(1 , 'Pratap' , 20 , 'male' , '123456789' , 'hazaribagh'),
    (2 , 'Ranjeet' , 24 , 'male' , '9876543210' , 'hazaribagh'),
    (3 , 'Abhishek' , 23 , 'male' , '9087654321', 'xyz' ),
    (4 , 'Deepak' , 24 , 'male' , '897654321' , 'xyz'),
    (5 , 'Rahul' , 26 , 'male' , '8689754321' , 'hazaribagh'),
    (6 , 'Vivek' , 20 , 'male' , '123456789' , 'hazaribagh')
);

# checking for default values
INSERT INTO students(id , name , age , gender , phone)   #here we don't add city , however the default value of city can be shown in city
VALUES(6 , 'Vivek' , 24 , 'male', '8976543213');


SELECT * FROM students;

 ```