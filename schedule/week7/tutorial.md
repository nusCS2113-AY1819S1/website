**An activity to do during tutorial:**<br>

<table>
<tr>
<td width="40%">

<include src="../../book/modeling/modelingBehaviors/sequenceDiagramsBasic/personListExercise.md" />

After that, draw a class diagram to match the code. Then, draw an object diagram to show the state of the objects after the code has executed one loop.

</td>
<td>
&nbsp;
</td>
<td>

<tip-box> 

Here are some sample diagrams to use as references:<br>
<img src="{{baseUrl}}/book/modeling/modelingBehaviors/sequenceDiagramsBasic/images/Machine.png" width="500"/>
<img src="{{baseUrl}}/book/modeling/modelingStructures/classDiagramsBasic/images/typicalClasssStructure.png" width="400"/><br>

</tip-box>

</td>
<tr>
</table>

**Questions to discuss during tutorial:**

<include src="../../book/modeling/modelingBehaviors/sequenceDiagramsIntermediate/q-essay-expainParserFactory.md" /><p/>

1. What is the profile of the target user of your product?. Describe the problem you are solving for that target user. Give some representative must-have user stories for your product that are not already present in <tooltip content="AddressBook-Level4">AB4</tooltip>.
1. What’s the use of assertions?
1. Demonstrate an assertion failure using Intellij.
1. What is a multi-level design? How is it used in AB4?
1. What is an API? How is it used in AB4?
1. Why do we need logging? What’s the purpose of logging levels? What are the available logging levels in AB4?
1. Explain what Gradle is. How is it used in AB4?
1. Explain what Travis is. How is it used in AB4?

{% from "schedule/index.md" import all_outcomes with context %}
{% from "common/tutorial.njk" import  show_week_evidences with context %}
{{ show_week_evidences("7", all_outcomes) }}