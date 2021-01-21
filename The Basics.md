NOTE: NOTES TAKEN AND ORGANIZED FROM *Data Structures and Algorithms in Java, 6th Edition_ International Student Version-Wiley (2014)*
## Modifiers
### Access Control Modifiers: public, protected, private
**public**:  
All classes may access the defined aspect. In Java, each public class must be defined in a separate file named classname.java, 
where “classname” is the name of the class (for example, file Counter.java for the Counter class definition).

**protected**:  
Access to the defined aspect is only granted to subclasses or classes in the same package. (TODO: package notes, link)

**private**:  
Access only granted to the same class.  
I assume different instances of the same class can access each other's private members.  
Wrote code and tested it. //TODO: push code to this repo.

### Other Modifiers: static, final, abstract
**static**  
Nothing different from C++(?) and Python(?).  
All instances share the same member.

**final**

If a variable is declared as final, it cannot be changed. If it's within a class, just declare it as static as well since it doesn't change anyways.

If a method is final, it cannot be overridden. If a class is final, it cannot be subclassed.

**abstract**  
Used for abstraction. A class with an abstract method must be an abstract class.  
- (How is it different from using interfaces?)
An interface has no concrete methods, while an abstract class can have concrete and abstract methods.  
- (Then how is an interface different from an abstract class with no concrete methods?)  
A class can implemenet multiple interfaces (multiple inheritance) but can only extend one abstract class.  
- (When should you use which?)  
When you need to inherit from multiple "parents", use interfaces. When you have a more concrete idea in mind what the class will be like, use abstract classes.
