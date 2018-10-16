**Show evidence of achieving v1.2 team/individual milestone**
* [One member] Show the 'insights' tab of your team repo's GitHub page
* [Each member] show these using the `master` branch in your computer:
  * Demo the enhancement you added to v1.2
  * Point out the part you added to the Developer Guide
   

### Questions to be discussed during tutorial

1. Does this code fragment compile? Why or why not?  
  ```java
  class A {
      void foo() {
          System.out.println("Foo from A");
      }
  }
  
  class B extends A {
      void foo() throws IOException {
          System.out.println("Foo from B");
      }
  }
  ```
2. Which method is statically bound which method is dynamically bound?
```java
class Animal {
    void eat() { 
        System.out.println("Eat food");
    }
}

class Dog {
    void eat() {
        System.out.println("Eat dog food");
    }
    
    void eat(String b) {
        System.out.println("Eat biscuit: " + b);
    }
}
```
3. Consider the diagram:<br>
<img src="{{baseUrl}}/book/architecture/architectureDiagrams/drawing/images/tip.png" height="190" /><br>
Which is a better design?
4. In the above diagram, what is the problem with the architecture diagram on the right?
5. IVLE quizzes allow a quiz to be attempted multiple times. For each attempt, it records the time taken. Model this scenario as a class diagram.
6. Draw another diagram to describe how you would implement the above it in code.
7. Give an example of defensive programming from AB4
8. What is the purpose of `@Before` and `@After` in JUnit?
9. What is the difference between decision and branch coverage?   

{% from "schedule/index.md" import all_outcomes with context %}
{% from "common/tutorial.njk" import  show_week_evidences with context %}
{{ show_week_evidences("9", all_outcomes) }}