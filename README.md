Download Link: https://assignmentchef.com/product/solved-cs2400-homework-7-book-class
<br>
Design classes, search strings, tokenizing strings, string member functions, and separate compilation.

<strong>Important: </strong>

<em>This is the first part of your final project. The Book class will be used in the second part of this project. <strong>Do not change the function names or their prototypes. Also, use the same file names given in the repository on GitHub (book.h, book.cc).</strong> </em>

<strong>You may use any function or library discussed in class or in the chapters we covered from your textbook. Do not use any other libraries or functions. </strong>

Design a class to keep track of a book. Each book has a <em>title</em>, <em>year</em>, and an <em>author</em>.  Your class must include the following constructors and functions (<strong>function names and prototype must match exactly</strong>):

<ul>

 <li>Book()</li>

</ul>

o A constructor that initializes a book to the default values: (“***”, 0, “***”).

<h1>• Book(string newTitle, int newYear, string newAuthor);</h1>

o A constructor that initializes a book’s title, year, and author to the specified parameters.

<h1>• Book(string allData)</h1>

o A constructor that splits the string specified (allData ) into the three book properties. The string is in the following format:

<h1>§ title|year|author</h1>

<ul>

 <li>Example:</li>

</ul>

“The Hitchhiker’s Guide to the Galaxy<strong>|</strong>1979<strong>|</strong>Douglas Adams”

<ul>

 <li>Setters (mutators) for all three member variables (e.g. setTitle)</li>

 <li>Getters (accessors) for all three member variables (e.g. getTitle)</li>

</ul>

<h1>• bool matchTitle(string targetTitle)</h1>

o Returns true if targetTitle is part of the book title o Using the example above it should return true if targetTitle is “galaxy”, “GUIDE tO”, “the hit”, etc.

<h1>• bool matchAuthor(string targetAuthor)</h1>

o Returns true if targetAuthor is part of the name of the lead author o Using the example above it should return true if targetTitle is “Doug”, “LAS”, “aDaMs”, etc.

<h1>• bool matchYear(string targetYear)</h1>

<ul>

 <li>Returns true if targetYear matches any part of the year.</li>

 <li>Using the example above it should return true if targetYear is “79”, “19”, or “1979” etc.</li>

</ul>

<h1>• bool match(string target);</h1>

o Returns true if target can be found any where in the book member variables § Using the example above it should return true if target is “97”,

“douglas”, “hitch”, etc.




<strong>Write a main program to test all the functions. </strong>

<strong> </strong>

<strong>Project Files:</strong>

Divide your project into three files:

<ul>

 <li>h

  <ul>

   <li>Contains the class definition</li>

  </ul></li>

 <li>cc

  <ul>

   <li>Contains the class implementation (all the functions)</li>

  </ul></li>

</ul>

<h1>• book_main.cc</h1>

o Main program to test your class <strong>Compiling your project: </strong>

<ol>

 <li>g++ -Wall -c book.cc

  <ul>

   <li>This creates the object file o</li>

  </ul></li>

 <li>g++ -Wall -c book_main.cc

  <ul>

   <li>This creates the object file o</li>

  </ul></li>

</ol>

<h1>3. g++ book.o book_main.o</h1>

<ul>

 <li>This creates the executable a.out</li>

</ul>




or

<h1>     g++ -Wall -std=c++11 -c book.cc book_main.cc</h1>

There is a Makefile provided to allow you to compile your program using the command:

<h1>          make</h1>




If you are using C++11 add the option –std=c++11 to your compile commands.




<strong>Hints: </strong>

<ul>

 <li>Start early. You may start by putting everything in one file and separate them later.</li>

 <li>Implement the getters, and setters functions first then start implementing the <em>match</em> functions one at a time. Test every function immediately after you write it.</li>

 <li>You may want to implement an output function to test your objects.</li>

 <li>Review the <em>string</em> They will be useful in this project.</li>

 <li>Write a function that converts a string to all lower case.</li>

 <li>The function stoi allows you to convert a string object to an integer. It requires compiling your program with -std=c++11 int x = stoi(“123”); will return the integer 123</li>

 <li>The function to_string converts a number to string. string s = to_string(123); will set s to the string “123”</li>

</ul>

<strong> </strong>

<ul>

 <li>For the third constructor, use the find and the substr string member functions.</li>

</ul>


