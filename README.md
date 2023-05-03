Download Link: https://assignmentchef.com/product/solved-cs1331-homework-03-file-reader
<br>



<strong> </strong>

<h1>Problem Description</h1>

Your company has a text file full of commands they don’t know how to execute. Now that they’ve hired you, they want you to do it! Write a program that takes in a text file via command line. This text file has a list of commands. Write a Java class, FileReader, that reads the file, follows the commands, and prints out the results.

<h1>Solution Description</h1>

The text file will need to be in the same directory as your FileReader.java file.

There are three possible commands in the text file. Each command will be followed by its arguments separated by spaces. There will always be the correct number of arguments. The arguments will always be the correct type (e.g. you will only get numbers for power, we will not give you a string like “hi”). The commands are allcaps, power, and substring.

<ul>

 <li>allcaps has one argument, a string that you will convert to uppercase. For example, the result of allcaps Hello would be HELLO. The string will always be one word.</li>

 <li>power has two arguments, a base and a power to raise that base to. For example, the result of power 2 3 would be 0</li>

 <li>substring has three arguments, a string, a start index, and an end index. For example, substring cs1331rocks 6 11 would result in rocks. The string will always be one word. The start index is inclusive, the end index exclusive. If either the start or end index is out of bounds, the result should be “Invalid command” instead of the substring.</li>

</ul>

You are encouraged to use methods in the <a href="https://docs.oracle.com/en/java/javase/11/docs/api/java.base/java/lang/String.html">Java String class</a> and the <a href="https://docs.oracle.com/en/java/javase/11/docs/api/java.base/java/lang/Math.html">Java Math class</a> to help you capitalize strings, calculate exponents, and create substrings.

For this assignment, you won’t be expected to write your own class. We have provided a FileReader.java file. In the main method, there will be a variable called commandsFile. You will use that variable to read from the file.

You will add three static methods, one for each command. public static String allCaps(String str) public static double power(int base, int power)

public static String makeSubstring(String str, int startIndex, int endIndex)

You will perform your computations in the method, then print the results from the main method. <strong>Again, don’t print anything from these methods, just from </strong><strong>main.</strong>

<h1>Testing your app</h1>

In order to test your program, you must compile by running javac FileReader.java in the same folder as FileReader.java

Then you can run java FileReader [fileName], providing some example file. The example file should be in the same directory as your program.

For example, if exampleFile.txt is

allcaps Hello power 2 3

substring cs1331rocks 6 11 substring hi 0 3

running java FileReader exampleFile.txt prints out

HELLO

8.0 rocks Invalid command

Remember that what you print out should match the defined output <em>exactly</em>. Deviation from what the output should be, even by a character or two, will result in lost points.

<h1>Rubric</h1>

<ul>

 <li>[15] correct printed output</li>

 <li>allcaps

  <ul>

   <li>[5] correct method signature &amp; return type</li>

   <li>[20] correct method output</li>

  </ul></li>

 <li>power

  <ul>

   <li>[5] correct method signature &amp; return type</li>

   <li>[20] correct method output</li>

  </ul></li>

 <li>makeSubstring

  <ul>

   <li>[5] correct method signature &amp; return type</li>

   <li>[20] correct method output</li>

   <li>[10] handles invalid start and end indices</li>

  </ul></li>

</ul>

<h1>Allowed Imports</h1>

To prevent trivialization of the assignment, you are <em>only </em>allowed to import java.util.Scanner, java.io.File, and java.io.FileNotFoundException.

<h1>Feature Restrictions</h1>

There are a few features and methods in Java that overly simplify the concepts we are trying to teach or break our auto grader. For that reason, do not use any of the following in your final submission:

<ul>

 <li>var (the reserved keyword)</li>

 <li>exit</li>

</ul>





