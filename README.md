# Polymorphism & Composition Homework - Quiz

# Polymorphism

1. What does the ___word___ 'polymorphism' mean?

    Being able to exist in multiple forms

2. What does it mean when we apply polymorphism to OO design? Give a simple Java example.

    An Object being able to be treated as different types

    ```
    public class Vehicle {
        // Class stuff
    }

    public class Car extends Vehicle {
        // Class Stuff
    }

    // Other Class
    Car car = new Car();

    ArrayList<Vehicle> vehicles = new ArrayList<>();vehicles.add(car);  
    ```

3. What can we use to implement polymorphism in Java?

    Inheritance and Interfaces can be used to implement polymorphism in Java.

4. How many 'forms' can an object take when using polymorphism?

    An object can be it's own class and also anything it inherits from or implements

5. Give an example of when you could use polymorphism.

    If you have a cakeshop that has many types of cake that all inherit from a Cake superclass, these can all be stored in the same typed collection and use any of the methods that are inherited without casting.



# Composition and Aggregation

6. What do we mean by 'composition' in reference to object-oriented programming?

    Composition is when an object is made up of other objects and these are owned by the object.

7. When would you use composition? Provide a simple example in Java.

    When an object contains other objects without which the object would cease to be a valid object

    ```
    public class House{
        private Roof roof;
        private Walls walls;

        public House(){
            this.roof = new Roof();
            this.walls = new Walls();
        }
    }
    ```

8. Give a difference between composition and aggregation?

    Aggregation is when objects are brought together but are not owned by the object, and the object could still exist without them.

9. What is/are the advantage(s) of using composition/aggregation?

    Aggregation allows the objects to be loosely coupled to the aggregatedobject, composition means they are totally part of the object

10. When using composition, when an object is destroyed, what happens to all the objects it is composed of?

    The objects are destroyed

11. When using aggregation, when an object is destroyed, what happens to all the objects it is composed of?

    The Objects live on
