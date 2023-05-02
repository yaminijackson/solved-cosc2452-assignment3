Download Link: https://assignmentchef.com/product/solved-cosc2452-assignment3
<br>
There is no book containing the music to every song that will be written. There is no book containing the answers to every mathematical calculation that we will need to perform. Similarly, there is no book, set of lecture slides, video, etc. that will give a programmer (you) the solutions to every programming problem. A programmer is able to take fundamental programming concepts and, with the experience they have gained from analysis, evaluation and problem solving, put them together to solve new problems.

A programmer is also a developer who can plan, minimise risks, iteratively develop, test and deliver programs to a “client”. As a part of this, a programmer should be able to show snapshots of the various stages of the development. The snapshot should be a runnable Java program that does not need to have all of the features that will be there in the final version of the program.

For this assignment, assume that you are a freelance programmer creating a small tool or a utility program of your own choosing to add to your portfolio of simple Java applications. With this project you aim to demonstrate to potential employers or clients how you can:

<ol>

 <li>Create a small tool or utility program using (exclusively) a limited set of fundamental code concepts.</li>

 <li>You are able to analyse and evaluate your implementations against possible alternatives in your code documentation.</li>

</ol>

<strong>Note: You must not just “throw in the concepts” to your program just because they need to be there; it should be clear from the code why a certain concept should be there and you must further explain these through your comments. You will also need debug your code on your own and document any issues, etc. You are given marks on your ability to fulfill all requirements of this document.</strong>

<strong>You can </strong>convert your Assignment 2 program to suit the requirements of Assignment 3.

If there are questions, you must ask via the Canvas→<a href="https://rmit.instructure.com/courses/67194/discussion_topics">Discussions</a>→Assignment 3 forum in a general manner (replicate your problem in a different context in isolation before posting). <strong>Do not show your assignment code to anyone</strong> as this could violate Academic Integrity requirements set by the University.

<ol start="2">

 <li>Assessment Criteria</li>

</ol>

<strong>This assessment will determine your ability to:</strong>

<ol>

 <li>Follow coding, convention and behavioral requirements provided in this document and in the lessons.</li>

 <li>Independently solve a problem by using programming concepts taught over the first several weeks of the course.</li>

 <li>Write and debug Java code independently.</li>

 <li>Document code.</li>

 <li>Ability to provide references where due.</li>

 <li>Meeting deadlines.</li>

 <li>Seeking clarification from your “supervisor” (instructor) when needed <u>via discussion forums</u>.</li>

 <li>Create a program by recalling concepts taught in class, understanding and applying concepts relevant to solution, analysing components of the problem, evaluating different approaches.</li>

</ol>

<ol start="3">

 <li>Learning Outcomes</li>

</ol>

This assessment is relevant to the following Learning Outcomes:

<ol>

 <li><strong><em>Demonstrate knowledge of basic concepts, syntax and control structures in programming</em></strong></li>

 <li><strong><em>Devise solutions to simple computing problems under specific requirements</em></strong></li>

 <li><strong><em>Encode the devised solutions into computer programs and test the programs on a computer</em></strong></li>

 <li><strong><em>Demonstrate understanding of standard coding conventions and ethical considerations in programming.</em></strong></li>

</ol>

<ol start="4">

 <li>Assessment details</li>

</ol>

<strong>Note: Please ensure that you have read sections 1-3 of this document before going further.</strong>

You must meet Functional Requirements (4.1), Code+Justification Requirements (4.2) and Documentation Requirements (4.3) to obtain the full mark for this assignment. You can also attempt the Bonus Requirements (4.4). You may receive 0 (zero) if you do not meet the submission requirements (see section 6).

4.1) Functional Requirements:

Important: The functional requirements below must be implemented and justified by following the 4.2 Code+Justification requirements.

F1) Allows the user to store an arbitrary number of records. May store more than 1 type of record.

F2) Allows the user to add, remove, modify such records.

F3) Allows the data for the records to be loaded from files and saved later in to a file.

F4) Has no restrictions on how many user interfaces can be used simultaneously in the system.

Tip: As you are not given marks for creativity or the usefulness of the program, do not spend too much time thinking of what is a

“good” program. What is good depends on how well the code is written, justified and documented (refer to sections 4.2 and 4.3).

<table width="688">

 <tbody>

  <tr>

   <td width="688">4.2) Code+Justification Requirements (20 marks):To receive marks for Code+Justification requirements, you must use the following Application.java template and code concepts to make a functionally cohesive program that also meets the functional requirements.</td>

  </tr>

  <tr>

   <td width="688"><strong>public</strong> <strong>class</strong> Application { <strong>private</strong> BackEnd backEnd; <strong>private</strong> FrontEndGTerm uiGT; <strong>private</strong> FrontEndConsole uiConsole;<strong>public</strong> Application() { <strong>this</strong>.backEnd = <strong>new</strong> BackEnd();<strong>this</strong>.uiGT = <strong>new</strong> FrontEndGTerm(<strong>this</strong>.backEnd); <strong>this</strong>.uiConsole = <strong>new</strong> FrontEndConsole(<strong>this</strong>.backEnd);}<strong>public</strong> <strong>static</strong> <strong>void</strong> main(String[] args) {Application <u>app</u> = <strong>new</strong> Application();}}</td>

  </tr>

 </tbody>

</table>




<table width="688">

 <tbody>

  <tr>

   <td colspan="3" width="688">The above file must not be changed by it should be possible to create multiple FrontEndGTerm objects to use the same BackEnd.Concepts must be used exclusively as demonstrated by Gayan’s weekly live lectures in this course offering. Code without justification in the given format would attract no more than 50% of the mark allocated for that component. Comments without code will not attract any marks.An important note on Java code validity: A program with even one red dot (compilation error) cannot be tested and therefore will attract 0 marks for the entire submission. Test your code thoroughly.</td>

  </tr>

  <tr>

   <td width="102"><strong>Code concept</strong></td>

   <td colspan="2" width="587"><strong>Code requirements below must also be justified as required</strong></td>

  </tr>

  <tr>

   <td width="102">CJ1) Muti classObject OrientedCode<strong>(0..6 marks)</strong></td>

   <td colspan="2" width="587">Requirements: +3 marks each for each + below when implemented as shown during Gayan’s live lectures+ Correctly uses the provided Application.java template to organise code by following OO concepts covered in main weekly live lectures by Gayan. (Application+BackEnd+FrontEndGTerm+FrontEndConsole and additional justifiable class(es) in the BackEnd) + Must create at least one more class to reduce code/logic duplication and have an array of this type in the BackEnd.Other deductions: -2 marks for each – below–                     The Application class submitted (the version provided in this document will be added by marker at time of marking) or has more than one class per submitted .java file.–                     Application class has been split further in to additional class(es).–                     One or more FrontEnd classes have been split further in to additional class(es).–                     GTerm or user interface mentioned outside of FrontEndGTerm class.–                     Scanner, System.out, System.err, etc. mentioned outside of FrontEndConsole class.–                     Has at least one object member variable that is not explicitly <em>private</em>.</td>

  </tr>

  <tr>

   <td width="102">CJ2) Other general <strong>(0..1 marks)</strong></td>

   <td colspan="2" width="587">Requirements: +0.5 marks each for each + below when implemented as shown during Gayan’s live lectures+ Descriptive identifier names which are relevant to their purpose. Follows naming conventions shown in lectures, other standard class materials and common ones in the Java API.+ Consistent formatting used. Comments and justifications start on the line before the documented block/statement (e.g. no in-line comments).Other deductions: -0.5 marks for each – below–                     Includes irrelevant or unreachable code+comments.–                     Uses break, continue, System.exit or similar branching anywhere in the code – Uses return in the middle of methods- Has at least one mention of <em>static</em>.–                     Has at least one mention of <em>static</em>.–                     Paths contain folders/slashes (e.g. addImageIcon, file I/O, etc.)</td>

  </tr>

  <tr>

   <td width="102">CJ3) Variables <strong>(0..1 marks)</strong></td>

   <td colspan="2" width="587">Requirements: +0.5 marks each for each + below when implemented as shown during Gayan’s live lectures + Demonstrates understanding of suitability of primitive data types vs. class.+ Declares variables in blocks where they need to be declared (avoids unnecessary “sharing” of  declarations)Other deductions: -0.5 marks for each – below– Uses variables when literals would have been suitable. – Uses literals when variables would have been suitable.</td>

  </tr>

  <tr>

   <td width="102">CJ4) Methods <strong>(0..1 marks)</strong></td>

   <td colspan="2" width="587">Requirements: +0.25 marks each for each + below when implemented as shown during Gayan’s live lectures + Each class has exactly one constructor+ Methods are created when absolutely necessary or when they reduce duplication of code. + Methods return values when suitable (e.g. accessor/get methods) + Methods take parameters when suitable (e.g. mutator/set methods).Other deductions: -0.25 marks for each – below–                     Not all object member variables, arrays, etc. declarations are explicitly initialised in this constructor before any other operations (e.g. there are no equal signs where member variables are declared).–                     Has examples of methods referring to an object member variable without using this. (“this dot”)</td>

  </tr>

  <tr>

   <td width="102">CJ5) User interface(FrontEnd…) classes<strong>(0..2 marks)</strong></td>

   <td colspan="2" width="587">Requirements: +1 marks each for each + below when implemented as shown during Gayan’s live lectures+ FrontEndGTerm uses GTerm exclusively for inputs and takes most, if not all, inputs via text fields/text areas/password fields (vs. getInputString). FrontEndGTerm uses GTerm exclusively for outputs and displays most, if not all, outputs within the GTerm window (as opposed to using .showMessageDialog…)+ FrontEndConsole uses Scanner’s .nextLine() exclusively for inputs (e.g. must not use other .next… methods).FrontEndConsole shows text-based menus and formats outputs in to tables, etc. as shown in weekly live lectures.Other deductions: -1 marks for each – below–                     FrontEnd… classes do not offer an identical set of functionalities to the end-user.–                     A FrontEnd… class has awareness of another FrontEnd class/object.–                     A FrontEnd… class has awareness of a custom class/object that should only be used by BackEnd (e.g. A FrontEnd must not communicate with a custom class type used by BackEnd’s primary array.) – Creates multiple Scanner objects.</td>

  </tr>

  <tr>

   <td width="102">CJ6) Conditional execution and repetition <strong>(0..1 marks)</strong></td>

   <td colspan="2" width="587">Requirements: +0.5 marks each for each + below when implemented as shown during Gayan’s live lectures+ Uses if/else/else if appropriately and exclusively for non-repeating conditional execution and at least one reachable else if statement.+ Uses while-loops appropriately and exclusively for repetition. Loop condition describes all situations under which the loop will repeat and condition fails eventually.Other deductions: -0.5 marks for each – below – Conditions include tautologies.– Redundant conditions.– Unreachable blocks.</td>

  </tr>

  <tr>

   <td width="102">CJ7) Arrays(not ArrayLists, etc.)<strong>(0..2 marks)</strong></td>

   <td colspan="2" width="587">Requirements: +1 marks each for each + below when implemented as shown during Gayan’s live lectures+ All array manipulation performed using loops, if-statements, etc. (as shown in weekly live lectures by Gayan)+ The size of the array mentioned in CJ1.Addition.2 should be able to vary at run-time. Run-time expansion allowed.Other deductions: -1 marks for each – below– Uses Arrays class– Uses System.arraycopy– Uses other classes (not covered in weekly live lectures) for array manipulation</td>

  </tr>

  <tr>

   <td width="102">CJ8) Fileinput+output fromBackEnd<strong>(0..6 marks)</strong></td>

   <td colspan="2" width="587">Requirements: +3 marks each for each + below when implemented as shown during Gayan’s live lectures + Allows the user to load records from file<u>s</u> specified at run-time. + Allows the user to save all data to a file specified at run-time.Other deductions: -1 marks for each – below – Does not use CSV when appropriate.– File reading code not in the most appropriate class.– File writing code not in the most appropriate class.– Does not use only BufferedReader+FileReader when reading.– Does not use only BufferedWriter+FileWriter when writing.– Keeps files open when not necessary to do so.</td>

  </tr>

  <tr>

   <td colspan="3" width="688"><strong>Justification Requirements</strong>Note: You will not receive full marks for the CJ requirements unless each occurrence is justified as required below.</td>

  </tr>

  <tr>

   <td colspan="2" width="120"><strong>Type of code</strong></td>

   <td width="568"><strong>Compare and justify your choice over other possible alternative…</strong></td>

  </tr>

  <tr>

   <td colspan="2" width="120">Declarations(also applies to class and method definitions)</td>

   <td width="568">Identifier names Data typesLocality of declaration (why object-level vs. parameter-level vs. method-level vs. block-level, etc.).</td>

  </tr>

  <tr>

   <td colspan="2" width="120">Contents of code blocks</td>

   <td width="568">Formulations (is there a simpler way to meet requirements without creating this code block?)Inclusions (what you have added and why?)Sequences (why are these in this order?)Exclusions (what you haven’t added and why)</td>

  </tr>

  <tr>

   <td colspan="2" width="120">Conditions</td>

   <td width="568">Formations of the logic</td>

  </tr>

  <tr>

   <td width="102"></td>

   <td width="18"></td>

   <td width="568"></td>

  </tr>

 </tbody>

</table>

<ul>

 <li>Documentation Requirements (5 mark penalty if not met):</li>

</ul>

Important note: Documentation must match with testable, functional and justified code to attract marks.

<strong><em>D1. Create an illustrated PDF user guide (one file). </em></strong>Must have <strong>side-by-side instructions</strong> on how to perform the same functionalities on both interfaces. Shows screenshots of sample inputs. Shows screenshots of corresponding sample outputs. Must include examples of using files to load and save. Include instructions on what the user can and cannot do (e.g. what they can and can’t input). Does not include any references to code as the guide is intended for a user who is not a programmer. This document needs to be professionally presented, more structured, starting with a table of contents, page numbers, clearly marked sections, etc.

<ul>

 <li>Bonus Requirements</li>

</ul>

Important note: The total mark of A1+A2+A3 is capped at 45 (for a full break-down, see Canvas→Assignments). To obtain any bonus marks, you need to be able to get full marks for the non-bonus/standard requirements of this assignment.

B1: Submit your final version of Assignment 3 one day before the deadline for +0.1 marks or 2 days before the deadline for +0.2 marks, etc.