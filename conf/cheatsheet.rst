Scripting Cheatsheet
====================

If you don't want to read through a bunch of documentation and are already quite
familiar with programming, you can read through this page and try getting started.

Useful Resources
----------------

Nashorn Engine
^^^^^^^^^^^^^^
 
`Nashorn <https://github.com/openjdk/nashorn>`_ is the javascript engine that 
is used to for scripting in Shimeji. No that is not a typo; it *is* javascript and 
not java. Javascript and java still are completely different languages but 
JavaScript can be run inside java.

When calling a function from xml, trying to access a non-existent or non-public 
function leads to an error. It is recommended to learn about Nashorn and its 
behavior since it has a few interesting quirks that are important for debugging 
(i.e print statements, accessors).

Keep in mind that ShimejiEE has a class filter that blocks access to all classes. 
This means java objects cannot be directly created from the scripts.

* `Nashorn javascript engine <https://docs.oracle.com/javase/10/nashorn/introduction.htm#JSNUG136>`_
* `interesting behavior of Nashorn <https://www.graalvm.org/reference-manual/js/NashornMigrationGuide/>`_
* `More interesting behavior of Nashorn <https://wiki.openjdk.java.net/display/Nashorn/Nashorn+extensions>`_

General JS & XML
^^^^^^^^^^^^^^^^

You'll have to figure out some JavaScript syntax. When editing the XML 
remember that you cannot use certain symbols (such as angle brackets) and will 
have to escape them.

* `Javascript MDN <https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide>`_
* `XML escape characters <https://stackoverflow.com/questions/1091945/>`_


Variables Overview
------------------

By default ``mascot`` is inserted into all script contexts. This represents the 
Mascot object that the script is controlling. 

// todo add the reference for the mascot object api

Types of Variables
^^^^^^^^^^^^^^^^^^

Repeating
"""""""""
``#{}``
Gets initialized the first time it's used and then refreshes 
the value periodically after that.

Stored
""""""
``${}``
Gets initialized the first time it's used and stores the value. Because it is not 
reset, this value can be changed by parts of the script.

Return Values
^^^^^^^^^^^^^
The returned value of a script is the value of the last statement that gets run.

A Warning about Initialization 
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

When relying on side effects of scripted variables to change the mascot, you need 
to make sure that the script is actually called! Since they are lazily initialized, just 
defining the variable is not enough.

If you are using a built-in variable (such as ``Condition``), the program will *usually* 
call the variable and therefore run the script. However it is is important to keep 
in mind that some action types don't call certain variables and/or call them at 
different times than other actions.

To get a sense for how the variables are called/run, you can use print statements and 
observe the output from the command line.

