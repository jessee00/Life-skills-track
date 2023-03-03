# <span style="background-color: black">Report on OOP:</span>

**Object-oriented programming (OOP) is a programming paradigm that emphasizes the use of objects and their interactions to design and build applications.**

OOP focuses on the objects that developers want to manipulate rather than the logic required to manipulate them. This approach to programming is well-suited for programs that are large, complex and actively updated or maintained. This includes programs for manufacturing and design, as well as mobile applications; for example, OOP can be used for manufacturing system simulation software.

OOP is based on the principles of encapsulation, inheritance, and polymorphism, which make it easier to manage complex codebases.

In this report, we will discuss these three principles of OOP and provide code samples to illustrate their usage in refactoring a difficult-to-manage codebase.
<br>

# <span style="background-color: black">**Encapsulation:**</span>
* Encapsulation is the concept of hiding the internal workings of an object from the outside world. 
* Encapsulation is a process of wrapping code and data together into a single unit, for example, a capsule which is mixed of several medicines.
* It is achieved by using access modifiers like private, public, and protected to restrict access to an object's properties and methods. 
* Encapsulation provides data security and helps maintain the integrity of the code.


<span style="background-color: black">Example:</span>

## java

```java
class Employee {

  private String name;
  private int id;
  private double salary;

  public void setName(String name) {
    this.name = name;
  }

  public String getName() {
    return name;
  }

  public void setId(int id) {
    this.id = id;
  }

  public int getId() {
    return id;
  }

  public void setSalary(double salary) {
    this.salary = salary;
  }

  public double getSalary() {
    return salary;
  }
}
```

In the above example, the Employee class has private properties like name, id, and salary. These properties can only be accessed through the public methods of the class, like setName, getName, setId, getId, setSalary, and getSalary. This ensures that the internal workings of the Employee object are hidden from the outside world.
<br><br>

# <span style="background-color: black">**Inheritance:**</span>

* Inheritance is the concept of creating a new class from an existing class. 
* The new class inherits all the properties and methods of the existing class and can also add its own properties and methods.
* Inheritance promotes code reusability and reduces code duplication.
* Inheritance represents the IS-A relationship which is also known as a parent-child relationship.

<span style="background-color: black">Example:</span>

## java

```java
class Animal {
  public void eat() {
    System.out.println("I can eat");
  }

  public void sleep() {
    System.out.println("I can sleep");
  }
}

class Dog extends Animal {
  public void bark() {
    System.out.println("I can bark");
  }
}
```

In the above example, the Animal class has two methods, eat and sleep. The Dog class extends the Animal class and adds its own method, bark. As a result, the Dog class has access to all the methods of the Animal class, as well as its own method.
<br><br>

# <span style="background-color: black">**Polymorphism:**</span>

* Polymorphism is the concept of using a single interface to represent multiple forms. 
* It allows objects of different classes to be treated as if they are objects of the same class. 
* Polymorphism is achieved through method overloading and method overriding.
* let's think of a superclass called Animal that has a method called animalSound(). Subclasses of Animals could be Pigs, Cats, Dogs, Birds - And they also have their own implementation of an animal sound (the pig oinks, and the cat meows, etc.).

<span style="background-color: black">Example:</span>

## java

```java
class Animal {
  public void makeSound() {
    System.out.println("Animal is making a sound");
  }
}

class Cat extends Animal {
  public void makeSound() {
    System.out.println("Cat is making a sound");
  }
}

class Dog extends Animal {
  public void makeSound() {
    System.out.println("Dog is making a sound");
  }
}
```

In the above example, the Animal class has a method called makeSound. The Cat and Dog classes override this method to provide their own implementation of makeSound. When a Cat or Dog object is created, the makeSound method of the corresponding class is called. This is an example of runtime polymorphism.
<br>

# <span style="background-color: black">Conclusion:</span>

* In this report, we have discussed the concepts of encapsulation, inheritance, and polymorphism in object-oriented programming.
* These concepts provide a modular approach to software development, making it easier to manage and modify code. 
* By using these concepts, we can create robust and scalable applications.  
<br>

# <span style="background-color: black">References:</span>

* [dotcms.com](https://www.dotcms.com/docs/latest/markdown-syntax#html-tags-%3Cblockquote%3E%3C-blockquote%3E) - Markdown syntax Editing.
* [Dre How-To](https://www.youtube.com/watch?v=DLLrcr9u_XI) - youtube channel for Markdown.
* [VS-code Studio DOCS](https://code.visualstudio.com/docs/languages/markdown) - For Editing.
* [setscholars.net](https://setscholars.net/java-tutorials-for-beginners-java-inheritance/) - Tutorials for java Inheritance.
* [beginnersbook.com](https://beginnersbook.com/2013/03/polymorphism-in-java/) - Polymorphism in Java.
* [educba.com](https://www.educba.com/encapsulation-in-java/) - Encapsulation in Java.
* [W3schools.io](https://www.w3schools.io/file/markdown-text-highlight/) - For Text & Background Editing.
* [techtarget.com](https://www.techtarget.com/searchapparchitecture/definition/object-oriented-programming-OOP) - For oops concepts.