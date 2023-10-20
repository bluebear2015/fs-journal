# CSharp and SQL Fundamentals
01. What is the purpose of a `namespace`?

  > | Namespaces help prevent naming conflicts and allow you to create a hierarchical structure for your code.|

02. What is the difference between a `class` and an `interface`?

  > | A class is a blueprint for creating objects. An interface is a contract that defines a set of members (methods, properties, events) that a class must implement. |

03. What is the method that returns an instance of a class, yet it has no return type?

  > | Constructors have the same name as the class and are used to initialize and create objects of the class. |

05. In the Car example what is the access modifier of the `Start()` method?

  ```c#
  abstract class Car
  {
    public string Start()
    {

      return "Vroooom";

    }
  }
  ```

  > |the constuctor the method is accessible from outside the class and from other classes that may derive from this abstract class.|

06. In the Car example what is `string` an indication of?

  > | it is the return type of the Start() |

07. In the Car example what is `abstract` preventing?

  > |preventing the Car class from being instantiated directly.|

08. In a SQL table, what is the difference between information in a row and information in a column?

  > | nformation in a row represents a specific data record, |

09. Demonstrate the necessary SQL for creating a table called `characters` with the values `name, age, description` as strings, and an `int` id.

  > | CREATE TABLE characters (
    id INT PRIMARY KEY,
    name VARCHAR(255),
    age VARCHAR(10),
    description VARCHAR(MAX)
); |

10. In SQL how can you query more than a single table? Provide an example.

  > | SELECT orders.order_id, customers.customer_name
FROM orders
INNER JOIN customers ON orders.customer_id = customers.customer_id; |
