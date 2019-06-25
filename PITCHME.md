# Why java was created?
* platform independent
* no pointers
* java has garbage collection

---

# Creating and destroying objects
* ways of creating object in java
* a = new A()
* a = new A(p, p)
* a = A.Builder(). .. .build()
* a = factory.createA()
* a = A.createA() 
* memory? - heap
* 3levels of memory for garbage collection
- Read `Gang of Four` Design patterns

---

# SFM
* may or may not create a new object
* - a class without a public constructor cannot be subclassed

# constructing with many params
* telescoping - can get very confising with lot of same tyupe of params
* using setter methods to set optional fields voilate immutability
* params to fucntions need to be immutable or make them synchronized
* string is immutable

# Singletons
* instantiated exactly once
* Implemented with
- public final Field
- SFM
- with Single Element Enum
* Serialization of singletons? first 2 months - implement readResolve - don't do it, instead implement with enum
---

# Avoid creating unnecessary objects
* Autoboxing creates unnescesary objects
* prototype factory pattern

# Common Object Methods
* Equals
* hashcode
* clone
* 






