# Intro to Server side concerns with JavaScript
01. What do the letters of the acronym `CRUD` stand for?

  > | Create Read Update Delete  |

02. Each action that `CRUD` represents maps to an HTTP request. What HTTP request does each `CRUD` action correspond to?

  > |Create = .create(), Read = .get(), Update = .post(), Delete = .remove / .delete |

03. What does `ORM` stand for? Which `ORM` do we use when interacting with MongoDB

  > | Object-Relational Mapping it is bridging our model to server.|

04. Which two `HTTP` request types include a body?

  > | Create Update|

05. In a/an _______ coding model, when you call a function, it returns only when the action has finished and stops your program for the time the action takes. Likewise in a/an _______ coding model, multiple things are allowed to happen at one time. When you perform an action, your program continues to run.  Fill in the blanks.

  > | sycncronis, Asyncronis |

06. What are the three types of data relationships? Provide an example of each.

  > | One-One, One-Many, Many-Many |

07. What is middleware?

  > | it is our server, that connects our backend to our database. |

08. The ______ pipeline delivers information from the client while the ______ pipeline returns it. Fill in the blanks. 

  > | Data, Data Processing|

09. Demonstrate the pattern that is used to include a request query with the client's `HTTP` request providing the property `tag` and the value `winter`.

  > |  dbcontext.tag.find(winter)|

10. What is a ***virtual property***?

  > | it is a scheme model that has access to other scheme models. |
