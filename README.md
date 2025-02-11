# Languages-and-Programming-Paradigms

What is Paradigm - a typical example or pattern of something ; in other words - a model .

So a programming Paradigm is a fundamental approach or style of programming that provides a set of principles, concepts, and techniques for designing and structuring software.
It helps in deciding how developers conceptualize and organize their code to solve the problems.

Programming Paradigms offer different methodologies for problem solving and code organization. some of them are below.

#### Imperative Programming (Non- Declarative Programming):
 <i> Fortran, C, Cobol, Pascal </i>
It focuses on describing how program operates , using statements that change a program's state . Developer writes code that specifies the exact steps the computer must take to accomplish a task.in short, we write instructions for the computer to follow it.

Imperative Approach to find the even numbers in the list.
```
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
even_numbers = []  # initializing an empty array 
for number in numbers:  # Loop 
    if number % 2 == 0: # check condition 
         even_numbers.append(number) # append to the list 
print(even_numbers) # output 
```


### Declarative programming :
<i> ML , Lisp, Haskel, Scheme </i>
This focuses on what the program should accomplish without specifying how it has to be achieved . We simply express the desired outcome without specifying how to achieve it.
we make use of some built-in functions to get the desired output.

Declarative Approach to find the even numbers in the list.
```
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
even_numbers = filter(lambda x: x % 2 == 0, numbers) # making use of built in functions 
print(list(even_numbers)) # convert t list and printing the numbers
```

### Object oriented programming :
 <i> C++, Java, C# ,Python </i>
Concentrates on structure code around the objects that encapsulates the methods and data associated with it , which helps in modularity and reusability.

```
class Car: #Define a Car class
    def __init__(self, make, model):
        self.make = make  # Car's make
        self.model = model  # Car's model

    def drive(self):
        print(f"The {self.make} {self.model} is driving!")


my_car = Car("Toyota", "Corolla")   # Create a Car object


my_car.drive()  # Output: The Toyota Corolla is driving!     # Call the drive method
```


### Logical Programming :
 <i> Prolog </i>
This helps in making formal logic to express the facts and rules . Program consists of logical statements primarily facts and rules—that define relationships and constraints within the system. 
The system then applies logical reasoning to these statements to derive conclusions or solve problems.


```
% Facts
parent(john, mary).     #  state that John is Mary's parent
parent(mary, susan).     # and Mary is Susan's parent.

% Rule
grandparent(X, Y) :- parent(X, Z), parent(Z, Y).  # defines that X is a grandparent of Y if X is a parent of Z and Z is a parent of Y.

% Query
?- grandparent(john, susan). # asks if John is a grandparent of Susan.

```
