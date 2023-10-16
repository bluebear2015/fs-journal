# A bit more CSharp and SQL
1. What does ***inheritance*** accomplish for us in C#?

  > | in C# allows a class, the derived or child class ,to inherit the characteristics and behaviors of another class. |

2. How does ***member inheritance*** work in C#? Does a `Class` inherit all members of the base `Class`?

  > | it allows a derived class to inherit all the non-private members of the base class. |

3. How does ***accessibility*** affect inheritance?

  > | affects inheritance by determining which members of a base class are accessible |

4. What is the difference between a `PRIMARY KEY` and a `FOREIGN KEY`

  > | a forgn key a column or a set of columns in a table that is used to establish a link between data in two tables. The FOREIGN KEY in one table refers to the PRIMARY KEY in another table. |

5. What is an ***alias***?

  > | a temporary name or identifier given to a table or column in a SQL query to make the query more readable |

6. Demonstrate how you would query a join statement that would get all of a doctors patients from the following collections:

  ```SQL
  CREATE TABLE doctors (
    id INT NOT NULL AUTO_INCREMENT,
    -- CODE OMITTED
    PRIMARY KEY (id)
  )

  CREATE TABLE patients (
    id INT NOT NULL AUTO_INCREMENT,
    -- CODE OMITTED
    PRIMARY KEY (id)
  )

  CREATE TABLE patient_doctors (
    id INT NOT NULL AUTO_INCREMENT,
    doctorId INT NOT NULL,
    patientId INT NOT NULL,

    FOREIGN KEY (doctorId)
      REFERENCES doctors(id),
    FOREIGN KEY (patientId)
      REFERENCES patients(id),
  )

  ```

  > |  ```SQL
   SELECT pat.*
   FROM doctors doc
   JOIN patient_doctors patdoc ON doc.id = patdoc.doctorId
   JOIN patients pat ON patdoc.patientId = pat.id
   WHERE doc.id = [Doctor's ID];
   ``` |

s
