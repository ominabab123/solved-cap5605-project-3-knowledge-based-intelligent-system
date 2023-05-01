Download Link: https://assignmentchef.com/product/solved-cap5605-project-3-knowledge-based-intelligent-system
<br>
<span class="kksr-muted">Rate this product</span>

For this project, you will design and build a knowledge-based intelligent system that collects user preferences and reasons about them.

1 Requirements

<ol>

 <li>The system should have an easy-to-use GUI (using the Python Tkinter module1) for collecting names of attributes and their values, hard constraints, and preferences. The system also should allow reading in these input from files. (See section 3 for formats of these files.)

  <ul>

   <li>Attributes (A) in this project are going to be binary.</li>

   <li>Hard constraints (H) are represented as propositional formulas in the Conjunc-tional Normal Form (CNF).</li>

   <li>The system should support preferences (T ) in the preference language of penaltylogic. Formulas involved in the preference theories are of CNF as well.</li>

  </ul></li>

 <li>The system should support the following reasoning tasks:

  <ul>

   <li>Existence of feasible objects: decide whether there are feasible objects w.r.t H, that is, whether there are models of H that are truth assignments making H true.</li>

   <li>Exemplification: generate, if possible, two random feasible objects, and show the preference between the two (strict preference or equivalence) w.r.t T .</li>

   <li>Optimization: find an optimal object w.r.t T .</li>

   <li>Omni-optimization: find all optimal objects w.r.t T .</li>

  </ul></li>

 <li>Thesystemshouldtakeadvantageoftheclaspsystem,aSATsolverthattakesapropo- sitional formula in CNF and computes its models. It can be used to compute feasible objects for H, check if a truth assignment satisfies a formula, etc. The short tutorial is on Canvas.</li>

 <li>For testing, the system should solve an instance, developed by you, that contains at least 6 hard constraints and at least 6 preference rules over at least 8 attributes. Also use this instance when demonstrating your system.</li>

</ol>

1See https://pythonspot.com/tag/tkinter/ and https://www.python-course.eu/ tkinter_labels.php for helpful references.

Dr. Xudong Liu University of North Florida School of Computing

CAP 4630/5605 – Spring 2019 Project 3 2

5. By Mar. 15 midnight, you will need to email me to discuss your progress. In your email, you will describe what you have done for this project and what you plan to do, and your questions if any. You will send me a screen shot of your GUI or at least a design of it, in case you will not have implemented in Python. Once I read your emails, I will respond with my comments to help you towards completing this project. Failure of this will result in deduction in the project grade. (See rubrics.)

2 Deliverables

Zip the following to name [your-last-name] Project3.zip and submit to Canvas.

1.

2. 3. 4.

3 3.1

A text file with description of the instance (attributes and their values, hard constraints, and preferences) you used for testing.

A directory that contains all your source codes.A README file that contains instructions to build and run your system.

APDFreportthatdescribeshowyoursystemworksandshowsthetestingresultsusing the test instance (e.g., screen shots of various steps).

File Formats Attributes File

<pre>appetizer:  soup, saladentree:  beef, fishdrink:  beer, winedissert:  cake, ice-cream...</pre>

3.2 Hard Constraints File

<pre>NOT soup OR NOT beerNOT soup OR NOT wine...</pre>

3.3 Preferences File