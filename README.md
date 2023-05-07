Download Link: https://assignmentchef.com/product/solved-kit103-assignment2-riding-the-sine-wave
<br>
<h1>Question 1: Riding the Sine Wave</h1>

The Fantastic Factorial Fun Park has a popular roller coaster (called the Sine Wave) with a somewhat complex set of rules for who can go on it. They have tasked you with writing a function that can tell people whether they can ride it or not. The function has three parameters: the person’s height in whole cm, age in whole years and a Boolean indicating if they are accompanied by an adult. It can return three possible string messages: ‘Sorry, you cannot ride’ if the rules exclude a person from riding the Sine Wave; ‘Find an adult’ if the person (child in this case) can ride as long as they come back with an adult; and ‘You can ride’ if they are allowed to ride the Sine Wave.

The rules are as follows:

Anyone less than 110cm or taller than 200cm cannot ride

Anyone younger than 6 cannot ride

If a child aged between 6 and 9 (inclusive) wishes to ride, they can do so if they are accompanied by an adult, otherwise they are told that they must ‘Find an adult’ Everyone else is allowed to ride the roller coaster

Your task is implement the rules above by completing the implementation of q1_sine_wave_check in the assignment script le. It is currently very pessimistic, telling all patrons that they are not allowed on. Complete the implementation by using any combination of if statements and Boolean expressions. The if statements may be nested as you see t.

Full marks will be given to solutions that use as few tests as possible. A solution that works for all cases, but which repeats a test or implements each rule completely separately, will get 1 mark. A solution that works for only many possible inputs will receive 0.5 marks, while a solution that works rarely or not at all will receive no marks.

Sample Test Data

<h1>Question 2: Implementing predicates as functions</h1>

There are stub (i.e., incomplete) implementations of each of these predicates as functions in the assignment script le (named q2_a through q2_d). Replace None in each of these stub functions with an implementation of the predicates below as they are written. The functions already have the required parameters listed. All parameters are Boolean.

<ol>

 <li>(*) ¬(a∧b)∧(a∨b)</li>

 <li>(*) a∨(¬b∨¬c∨¬d)</li>

 <li>(a∨b)∧(a∨c)</li>

 <li>a∧¬a</li>

</ol>

<h1>Question 3: Simplifying predicates</h1>

For each subpart (a)–(d) in Question 2, write a simpli ed implementation. There are stub functions named q3_a through q3_d for you to complete. KMA155 students must attempt at least parts (a) and

(b).

<h1>Question 4: The Letter Detector</h1>

The ACME Logic Company has a simple object recognition system that can identify when a particular arrangement of horizontal and vertical lines represents a letter (not which letter, only that it is a letter). They have a camera that can detect four di erent lines: horizontal lines either at the top or bottom of an image, and vertical lines at the left or right. Although the image may be hand-drawn, their detector ‘sees’ it as if it were like part of a digital display, like this: a

d      b

c

To determine if the arrangement of lines looks like a letter they use the following truth table (for convenience the truth table is presented using 0 for False and 1 for True, but the function accepts four Boolean variables a–d and returns a Boolean value). The Letter column is only for information; the function will not attempt to actually identify the letter.

<table width="330">

 <tbody>

  <tr>

   <td width="37">a</td>

   <td width="37">b</td>

   <td width="37">c</td>

   <td width="37">d</td>

   <td width="95">Output</td>

   <td width="87">Letter</td>

  </tr>

  <tr>

   <td width="37">0</td>

   <td width="37">0</td>

   <td width="37">0</td>

   <td width="37">0</td>

   <td width="95">0</td>

   <td width="87"> </td>

  </tr>

  <tr>

   <td width="37">0</td>

   <td width="37">0</td>

   <td width="37">0</td>

   <td width="37">1</td>

   <td width="95">1</td>

   <td width="87">I</td>

  </tr>

  <tr>

   <td width="37">0</td>

   <td width="37">0</td>

   <td width="37">1</td>

   <td width="37">0</td>

   <td width="95">0</td>

   <td width="87"> </td>

  </tr>

  <tr>

   <td width="37">0</td>

   <td width="37">0</td>

   <td width="37">1</td>

   <td width="37">1</td>

   <td width="95">1</td>

   <td width="87">L</td>

  </tr>

  <tr>

   <td width="37">0</td>

   <td width="37">1</td>

   <td width="37">0</td>

   <td width="37">0</td>

   <td width="95">1</td>

   <td width="87">I</td>

  </tr>

  <tr>

   <td width="37">0</td>

   <td width="37">1</td>

   <td width="37">0</td>

   <td width="37">1</td>

   <td width="95">0</td>

   <td width="87"> </td>

  </tr>

  <tr>

   <td colspan="4" width="148">a          b          c            d</td>

   <td width="95">Output</td>

   <td width="87">Letter</td>

  </tr>

  <tr>

   <td width="37">0</td>

   <td width="37">1</td>

   <td width="37">1</td>

   <td width="37">0</td>

   <td width="95">0</td>

   <td width="87"> </td>

  </tr>

  <tr>

   <td width="37">0</td>

   <td width="37">1</td>

   <td width="37">1</td>

   <td width="37">1</td>

   <td width="95">1</td>

   <td width="87">U</td>

  </tr>

  <tr>

   <td width="37">1</td>

   <td width="37">0</td>

   <td width="37">0</td>

   <td width="37">0</td>

   <td width="95">0</td>

   <td width="87"> </td>

  </tr>

  <tr>

   <td width="37">1</td>

   <td width="37">0</td>

   <td width="37">0</td>

   <td width="37">1</td>

   <td width="95">0</td>

   <td width="87"> </td>

  </tr>

  <tr>

   <td width="37">1</td>

   <td width="37">0</td>

   <td width="37">1</td>

   <td width="37">0</td>

   <td width="95">0</td>

   <td width="87"> </td>

  </tr>

  <tr>

   <td width="37">1</td>

   <td width="37">0</td>

   <td width="37">1</td>

   <td width="37">1</td>

   <td width="95">1</td>

   <td width="87">C</td>

  </tr>

  <tr>

   <td width="37">1</td>

   <td width="37">1</td>

   <td width="37">0</td>

   <td width="37">0</td>

   <td width="95">0</td>

   <td width="87"> </td>

  </tr>

  <tr>

   <td width="37">1</td>

   <td width="37">1</td>

   <td width="37">0</td>

   <td width="37">1</td>

   <td width="95">0</td>

   <td width="87"> </td>

  </tr>

  <tr>

   <td width="37">1</td>

   <td width="37">1</td>

   <td width="37">1</td>

   <td width="37">0</td>

   <td width="95">0</td>

   <td width="87"> </td>

  </tr>

  <tr>

   <td width="37">1</td>

   <td width="37">1</td>

   <td width="37">1</td>

   <td width="37">1</td>

   <td width="95">1</td>

   <td width="87">O or D</td>

  </tr>

 </tbody>

</table>

You have two tasks:

<ol>

 <li>(*) Transfer the information in the truth table to the Karnaugh map stored in q4_kmap in the script le, treating the columns as ab and rows as cd. q4_map is a list of lists, but you can treat it as if it were a table: replace the appropriate locations with 1s. Tip: Draw the Karnaugh map on paper rst and identify the groups. You won’t be able to show the groups in the script le, but this will help with part (b). (0.5 marks)</li>

 <li>(*) Replace the complicated Boolean expression currently in q4_acme_letter_detector with a simpli ed expression determined from your Karnaugh map. (1 mark)</li>

</ol>