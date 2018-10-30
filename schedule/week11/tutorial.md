**Show evidence of achieving v1.3 team/individual milestone**

**Demo**
* We will do a timed demo this week.
* Demo your product for v1.3 using the jar file from GitHub.
* Two or three members do the demo of the entire product. 
  
**Questions to discuss during tutorial**
-	What does OODM model?
-	What is gray box testing?
-	Explain: Equivalence Partitioning improves E&E of testing
-	What are the EP for `day` parameter?
```java
/** 
 * Returns true if the three values represent a valid day
 */
boolean isValidDay(int year, int month, int day) { … }
```
-	Explain: Boundary Value Analysis improves E&E of testing
-	What are boundary values for the parameter `day`?
- 	Apply heuristics for combining multiple test inputs to improve the E&E of the following test cases, assuming all 6 values in the table need to be tested. Italics indicate invalid values. Point out where the heuristics are contradicted and how to improve the test cases. <br>
SUT: `consume(food, drink)`

|    Test   Case    |    Food           |    Drink     |
|-------------------|-------------------|--------------|
|    TC1            |    Rice           |    Soda      |
|    TC2            |    Ice   cream    |    _Poison_  |
|    TC3            |    _Stone_        |    _Acid_    |

- Which process do we use in the project?
- Distinguish between breadth-first and depth-first iterative processes using your project as an example.
- Relate agile process to the project


{% from "schedule/index.md" import all_outcomes with context %}
{% from "common/tutorial.njk" import  show_week_evidences with context %}
{{ show_week_evidences("11", all_outcomes) }}