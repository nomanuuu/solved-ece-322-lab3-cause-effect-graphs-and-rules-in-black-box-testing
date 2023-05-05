Download Link: https://assignmentchef.com/product/solved-ece-322-lab3-cause-effect-graphs-and-rules-in-black-box-testing
<br>
The objective of this laboratory experiment is to become familiar with the use of cause-effect graphs and rules in black box testing, and to learn how these tools can be used to great effect in test case generation.

Introduction

The following sections will serve as an introduction to the testing technique used in this lab

<strong>Cause-Effect graphs </strong>

<ul>

 <li>Restates the software’s requirements in terms of logical relationships between inputs and outputs</li>

 <li>Represents the results as a boolean graph, called a cause-effect graph. This graph shows the relation between inputs and outputs in a logical manner.</li>

 <li>Provides a systematic view to design functional test cases from requirement specifications</li>

 <li>Can be used to significantly reduce the number of required test cases</li>

 <li>Refer to the lecture notes for instructions on using cause effect graphs and decision tables to generate test cases.</li>

</ul>

<strong><u>Preparation:</u></strong>

Prepare a set of test cases for all tasks you will be completing during the lab session. Follow formatting for test cases similar to the formatting used in lab 1 and 2. As before, only test cases for the testing strategies relevant to this lab need to be defined.

<h1>Lab Experiment</h1>

<strong>Task 1</strong>

The requirements of a simple car insurance premium program can be concisely expressed as a cause-effect graph/set of logical rules. The rules are based on the rationale that when a client has not made any claims, their insurance premium can be lowered due to small risk. As well, the age and gender of the client are variables to consider when deciding the final premium to charge. The rules that satisfy the system requirements for calculating the car insurance premium are given by the following set of rules:

IF sex = Male AND age &lt; 25 AND claims = 0 THEN premium = $1500

IF sex = Male AND 25 ≤ age &lt; 65 AND claims = 0 THEN premium = $1000

IF sex = Female AND age &lt; 65 AND claims = 0 THEN premium = $750

IF age ≥ 65 AND claims = 0 THEN premium = $1500

IF claims ≥ 1 THEN premium = $3000

The input variables are sex, age, and claims; however, these are not the causes of the system: the conditions of the inputs are the causes. Likewise, the effect of the system is the condition of the output variable premium. The causes and effects are given in the following table.




<table width="602">

 <tbody>

  <tr>

   <td width="300">Causes</td>

   <td width="301">Effects</td>

  </tr>

  <tr>

   <td width="300">A.  sex = MaleB.  sex = FemaleC.  age &lt; 25D.  25 ≤ age &lt; 65E.  age ≥ 65F.   claims = 0G.  claims ≥1</td>

   <td width="301">Y1. premium = $750Y2. premium = $1000Y3. premium = $1500Y4. premium = $3000 </td>

  </tr>

 </tbody>

</table>




The rules can be expressed them in terms of causes and effects expressions by analyzing the rules to form intermediate and causal nodes.

<strong>Your task</strong>​ for this section is to:

(1) Create the cause effect graph for the car insurance premium system described by  the above rules

<ul>

 <li>Generate a decision table for the system from the cause effect graph</li>

 <li>Develop test cases using the decision tables as shown in the lecture notes</li>

 <li>Evaluate the set of test cases against the provided lab application. Record your results, and identify any test failures.</li>

</ul>

For ​<strong>your report</strong>​:

<ul>

 <li>Provide a test case table, in the same format as in previous labs. Test cases must always be presented in a table format with clear descriptions, expectations and results.</li>

 <li>Provide a discussion on the effectiveness of cause effect graphs in the generation of a minimal set of test cases. Compare this method to previous testing methods explored in this course. How well were the number of test cases reduced? Are the tests more effective? More efficient? Are there cases this type of testing misses?</li>

 <li>Comment on the effectiveness of the testing method, did you discover any failures in the application? Do the tests do a good job of covering the applications functionality in your opinion? Keep in mind that not finding errors does not indicate poor tests, nor does finding errors indicate good tests.</li>

</ul>

<strong>Task 2 </strong>

A boiler shutdown control system is described in the control flow graph in the figure below. The system consists of 8 internal sensors (inputs A through H) and 2 external shutdown controls (I, and J). The internal sensors detect failures in meters, pumps and other systems. The cause effect graph is used to describe a system that determines whether or not the boiler should be shut down in certain scenarios.

<em>Figure shows decision tree of the boiler system “/” is an OR, “/” is an AND. </em>

<em> *[1] Paradkar A., Tai K.C., Vouk M.A., Specification-based testing using cause-effect graphs, Annals of Software Engineering, vol. 4, 1997, pp. 133-157. </em>

<strong>Your task</strong>​ for this section is to:

(1) Determine the cause effect rules for the boiler shutdown system as derived from the above control flow graph. These rules should be simple rules which can easily be transformed into test cases. Avoid the use of too many logical conjunctions. (2) Generate decision tables for the system on the basis of your derived rules.

<ul>

 <li>Develop test cases using the decision table as shown in lecture</li>

 <li>Execute your test cases for the provided lab application, and record your results. As before test cases should be presented in a readable, clean test case table.</li>

</ul>

For ​<strong>your report</strong>​:

<ul>

 <li>Include your test case table with meaningful descriptions, and clear expectations and results. Any failed test cases should be highlighted.</li>

 <li>Draw conclusions on the use of this method from your experiments. Similar to</li>

</ul>

Task 1, comment on the effectiveness, efficiency etc of cause effect graphs/logical rules and discuss their effectiveness in comparison to methods used in past labs, and to combinatorial testing.

<strong>Lab report: </strong>

Must be typed, no handwritten versions will be accepted. Follow the general format as included in the lab guideline. Your report should include:

<ul>

 <li>Your write-up and​<strong> all graphs/tables</strong>​ required for the tasks</li>

 <li>The results of your test cases in table form</li>

 <li>Any conclusions you have drawn from these test cases regarding the applications under test.</li>

 <li>Your discussion on the testing methods and their effectiveness</li>

</ul>