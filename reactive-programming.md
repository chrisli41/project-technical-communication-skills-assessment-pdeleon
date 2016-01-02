#Reactive Programming  
  
---  

### Reactive vs. Imperative

In order to understand Reactive programming lets begin with imperative programming. So in imperative programming when `a = b + c`  is evaluated, `a` is assigned the result of `b + c`. And later the values of `b` and `c` can be changed without effecting the value of `a`.  

```
var b = 10;
var c = 5;

var a = b + c;

console.log(a); // displays 15

var b = 5;
var c = 2;

console.log(a); // displays 15
```
  
Reactive programming is the opposite. So what is reactive programming? Reactive programming (RP) is a style of programming based on code that automatically reacts to changes. For example, in Reactive programming, the value of `a` would automatically be updated based on the new values.    

```
var b = 10;
var c = 5;

var a = b + c;

console.log(a); // displays 15

var b = 5;
var c = 2;

console.log(a); // displays 7
```
Reactive programming is like a modern spreadsheet program. In a spreadsheet program it's cells can contain values or formulas that are evaluated based on other cells. Whenever the value of the other cells change, the value of the formula is automatically updated.    
   
### Key Points of Reactive Programming

- Reactive programming can range from very explicit (more reactive) to very implicit (more imperative/functional). And can be purely static, or dynamic.

- Higher-order reactive programming uses data flows to create other data flows and uses the same evaluation as the first. 

- Differentiated reactive programming gives different parts of data flow different evaluation priorities. Like a word processor, the making of a spelling error does not need to be in sync with the insertion of characters. The spell checker is given a lower priority, allowing it to be delayed while keeping other data-flows instantaneous.

- Functional reactive programming (FRP) combines reactive programming and functional programming, and has been used for programming graphical user interfaces (GUIs), robotics, and music.

- Object-oriented reactive programming (OORP) is a combination of object oriented programming and reactive programming.

- Reactive programming has similarities with the observer pattern commonly used in object-oriented programming. For example, the observer pattern commonly describes data-flows between whole objects/classes, whereas object-oriented reactive programming could target the members of objects/classes.

- Reactive programs are not necessarily evaluated the same way stack based programming languages are. All data, that is taken partially or completely from the data that was changed, reacts to the change. The most natural way to achieve this is an invalidate/lazy-revalidate scheme. Keep in mind that most computations that would be evaluated and forgotten in a normal programming language need to be represented in memory as data-structures.
