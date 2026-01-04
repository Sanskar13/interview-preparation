**Creational Design Pattern**:
    * Factory -> You create a factory, which gives you the object. This helps

        * Helps you avoid modification at multiple places for a particular object, like creating "new Car()" at 15 places and changing in case a new parameter need to be added, simply create VehicleFactory (or whatever interface name is, that factory) and use it to return the instance, this way you don't change at multiple places only a single place of modification.
        *Change at 1 place-> changes everywhere in application, like car has a engine now, so just change in factory like new car(new engine())*
        
        *  you can always add a new vehicle in a factory below all classifications and use it. 

        ADV: Centralized factory for object creation, Scalability due to new additions of object creations, maintainable due to modification at one place itself.

        Real life use-cases: DB connections, 

        <mark>Any object creation, where there can be different types of object creation -> we can use factory</mark>
        <mark>Factory simplifies object creation in a centralized places, Makes application extendible, scalable and more maintainable, Best suited for places where there are variety of objects, Ensures we can add new types or change instantiation logic without modifying client code</mark>