**Primitive Data Type**

| Logical      | boolean(true/false)                                           |
|--------------|---------------------------------------------------------------|
| Textual      | char(16-bit Unicode character)                                |
| Integers     | byte(1 byte), short(2 bytes), int(4 bytes) and float(4 bytes) |
| Real numbers | double(8 bytes) and float(4 bytes)                            |

**Introduction to Object-oriented programming(OOP)**

| Classes                                                                                               | = a model for creating objects. Objects (also called “instances”) can be created after the class is defined. A program can only contain one copy of each class, but can have many objects.        |
|-------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Objects                                                                                               | = entities other than the primitive data type e.g. String, Scanner, File, PrintWriter, Exceptions, Arrays, etc.                                                                                   |
| Classes/Objects can define: variables inc. instance variables(attributes) and local variables methods |                                                                                                                                                                                                   |
| Attributes (instance variables)                                                                       | = variables that belong to a class. created when an class/object is created. declared outside of any methods. can be accessed by any method of the object(or even other objects if it is public). |
| Local variables                                                                                       | = variables that declared inside methods. created each time when the method is called. destroyed when exited from an object. can be used inside the method only.                                  |

**Arrays (Vectors/Tuples in mathematics)**

| Definition      | = a linear collection of items stored at contiguous memory locations.                                                                                                                                                                                              |
|-----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Characteristics | Items are of the same type. Position is calculated by adding an offset to the base value (i.e. first address). Memory are statistically allocated when declared (i.e. no expanding or shrinking).                                                                  |
| Complexity      | Time = O(n) [O(1) for accessing an element] Memory = O(1) [constant once declared]                                                                                                                                                                                 |
| Advantages      | Allows random access to elements, faster accessing time. have better cache locality (i.e. the tendency to access the same set of memory locations repetitively over a short period of time.). represents multiple data items of the same type using a single name. |
| Limitations     | The size of the array is unchangeable to prevent the risk of overwriting other data. Memory spaces are determined by the array size instead of the numbers of elements. Have to move half of the elements for each insertion or deletion on average.               |
| Examples        |                                                                                                                                                                                                                                                                    |

**Linked List**

| Definition      | = a linear collection of items stored and linked using pointers.                                                                                                                                 |
|-----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Characteristics | represented by a pointer to the first node(the head) of the linked list. Each node consists of two parts: data (store integer, strings or any type of data). pointer/reference to the next node. |
| Complexity      | Time: O(n) [O(1) for insertion and deletion] Space: O(n)                                                                                                                                         |
| Advantages      | Allows dynamic size and can allocate memory in runtime. Useful when the size is uncertain and large variation in array sizes. Ease of insertion and deletion.                                    |
| Disadvantages   | Have to access elements sequentially from the first node and thus worse cache locality. Extra memory space for a pointer.                                                                        |
| Examples        |                                                                                                                                                                                                  |

**Stacks**

| Definition      | = linear order data structures that store objects in a default LIFO (Last In First Out) structure.                                                                                                                                                                                                                                       |
|-----------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Characteristics | Allows four main operations/methods: Push: puts a new value on the top of a stack. Pop: takes a value from the top of a stack. Peep: returns at the top element without removing it. IsEmpty: checks if the stack is empty and return true/false. Reverse Polish Notation (RPN) = all operators are expressed after the second operands. |
| Complexity      | Time: O(n) [O(1) for insertion and deletion] Space: O(n)                                                                                                                                                                                                                                                                                 |
| Advantages      |                                                                                                                                                                                                                                                                                                                                          |
| Disadvantages   |                                                                                                                                                                                                                                                                                                                                          |
| Examples        |                                                                                                                                                                                                                                                                                                                                          |

**Queues**

| Definition      | = linear data structures that store objects in a FIFO (First In First Out) structure.                                                                                                                                                                                                                  |
|-----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Characteristics | Allows four main operations/methods: Enqueue: inserts a new element at the rear of a queue. Dequeue: deletes and returns the element at the front of a queue. Front: gets the front item from queue. Rear: gets the last item from queue. Types in Java: ArrayBlockingQueue, PriorityQueue, LinkedList |
| Complexity      | Time: O(n) [O(1) for insertion and deletion] Space: O(n)                                                                                                                                                                                                                                               |
| Advantages      |                                                                                                                                                                                                                                                                                                        |
| Disadvantages   |                                                                                                                                                                                                                                                                                                        |
| Examples        |                                                                                                                                                                                                                                                                                                        |

**Binary Tree**

| Definition      | = hierarchical data structure that store objects in parent(root)/children relationship.                                                                                                                                                                     |
|-----------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Characteristics | especially suitable for information that naturally forms a hierarchy. Maximum number of nodes at level ‘l’ is 2\^l. Maximum number of nodes of height ‘h’ is 2\^h -1. Minimum possible height or the minimum number of levels is log\^2(n+1), with n nodes. |
| Complexity      |                                                                                                                                                                                                                                                             |
| Advantages      | Allows dynamic size and can allocate memory in runtime.  provides moderate access/search (faster than Linked List and slower than Arrays). provides moderate insertion/deletion (quicker than Arrays and slower than Unordered Linked Lists).               |
| Disadvantages   |                                                                                                                                                                                                                                                             |
| Examples        |                                                                                                                                                                                                                                                             |

**Hash Tables**

| Definition      | = an improved direct access table with hash function.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
|-----------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Characteristics | The “value” can be any date type or objects. Hash function = converts a given big number to a small practical integer value that can be used as index in hash table. cannot control the order and the position when the entries are actually stored. hashcode = hashcode\*MULTIPLIER + (int)[String].charAt([index]) The initial value of the hashcode = 0. MULTIPLIER is usually a power of 2 for faster computation. return hashcode % ([tableSize]-1) generates a hash code between 0 and tableSize-1. Two considerations: Efficiently computable. Should uniformly distribute the keys. Hash table = an array that stores pointers to record corresponding to the given big number. Collision handling = situation where a newly inserted key maps to an already occupied slot in hash table. Chaining = makes each cell of a hash table point to a linked list of records that have same hash function value. buckets = the memory location represented by hash codes in a hash table. by using the overloading method. Open Addressing = stores all elements in the hash table, each entry then contains either a record or NIL. Load Factor λ = *N*entries / *N*buckets Too few buckets(large Load Factor) would lead to more collisions. Enumeration = a complete, ordered listing of all the items in a collection. use hasMoreElements() and nextElement() functions to loop through all keys. Rehashing = Increase the *N*buckets and re-enter all keys when the table is too compacted. is done automatically in Java. |
| Complexity      | Time: O(1) - O(n) [for all access, search, insertion and deletion] Space: O(n)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| Advantages      |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| Disadvantages   |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| Examples        |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |