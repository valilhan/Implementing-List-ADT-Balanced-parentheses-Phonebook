Data Structures and Algorithms
IT University Innopolis
        - Spring
     - Assignment
1 About this homework Contents
1.1 Coding part
1.1.1 Preliminary tests
1.1.2 Code style and documentation
1.2 Theoretical part
1.3 Submission
2 Coding part
2.1 Implementing List ADT
2.2 Balanced parentheses
2.3 Phonebook
3 Theoretical part
3.1 Big O notation
3.2 Hashing
1 About this homework Contents
1.1 Coding part
For practical (coding) part you have to provide you program as a single Java
class file that contains all necessary definitions and amainmethod.
The program should read from standard input and write to standard output
unless mentioned otherwise.

1.1.1 Preliminary tests
For some coding parts a CodeForces or CodeTest system will be used for
preliminary tests. You will have to specify a submission number in those
systems as a proof that your solution is correct. Only correct solutions will
be assessed further by TAs.
1.1.2 Code style and documentation
The source code should contain adequate internal documentation in the form
of comments. Internal documentation should explain how the code has been
tested, e.g. the various scenarios addressed in the test cases.

Do not forget to include your name in the internal documentation.
All important exceptions should be handled properly.

Bonus points might be awarded for elegant solutions, great documentation
and the coverage of test cases. However, these bonus points will only be able
to cancel the effects of penalties.
1.2 Theoretical part
Solutions to theoretical exercises have to be elaborate and clear. Write all
solutions in a single document and make it a PDF for submitting.
Do not forget to include your name in the document.
1.3 Submission
You are required to submit your solutions to all parts via Moodle.

For this assignment you will need to submit:

Java class file(s) for the coding parts;
link(s) to accepted submission(s) in CodeForces as a proof of correctness;
a PDF file with solutions for theoretical parts.
Submit files as a single archive with your name and group number. E.g.
BS18-00_Ivanov_Ivan.zip.

2 Coding part
2.1 Implementing List ADT
Implement the List ADT using both Dynamic-Array and Doubly-Linked-List
implementations. Implementations should be generic and support storing
elements of arbitrary types.
Note: you can declare List ADT in Java as either an interface or an abstract
class.

The List ADT should support the following operations:

isEmpty()— check if the list is empty;
add(i, e)— add elementeat positioni;
addFirst(e)— add elementeto the start of the list;
addLast(e)— add elementeto the end of the list;
delete(e)— delete elementeif it exists in the list;
delete(i)— delete element at positioni;
deleteFirst()— remove the first element from the list;
deleteLast()— remove the last element from the list;
set(i, e)— replace element at positioniwith new elemente;
get(i)— retrieve element at positioni.
Both implementations should provide clear documentation for every method,
including time complexity using big- O orΘnotation.
For doubly-linked list implementation you can choose to use sentinel or not.
2.2 Balanced parentheses
Implement a program that reads a sequence of tokens and determines whether
parenthesis (()), brackets ([]) and braces ({}) are properly balanced.
If input sequence has properly balanced delimiters then just output
Input is properly balanced.
Otherwise your program should specify the problematic location (line and
column numbers) in the input and what symbol was expected. For example
for this input
function random () {
return 4]
}
Your program should output this message:

Error in line 2, column 11: expected '}', but got ']'.
In this exercise you are allowed to reuse Stack implementation from labs or
implement a new one from scratch.
2.3 Phonebook
Write a program that manages a phonebook. Input for your program is a
series of commands. Every command can either update the phonebook or
query it:

ADD ,— add a phone number to
contact; the contact should be created if not exists;
examples:
- ADD Ivan Ivanov,+
- ADD Bro,
- ADD Ivan Ivanov,+
DELETE — delete entire contact from the phonebook;
examples:
- DELETE Ivan Ivanov
DELETE ,— delete a specific phone number
from a contact; if a contact does not exist or it does not have specified
phone number — do nothing; examples:
- DELETE Ivan Ivanov,+
FIND — lookup contact info; this is the only command
that has output:
- if contact is not found (or has no associated phone numbers) output
No contact info found for , e.g.:
FIND Petr Petrov
No contact info found for Petr Petrov
- otherwise output all phone numbers associated with the contact,
e.g.:
FIND Ivan Ivanov
Found 2 phone numbers for Ivan Ivanov: +71234567890 +
3 Theoretical part
3.1 Big O notation
Prove or disprove the following statements using the definition of big O
notation:
n
2
3 −^3 n = O ( n
(^2) )

k 1 n^2 + k 2 n + k 3 = O ( n^2 )
3 n = O (2 n )
0_._ 001 n log n − 2000 n + 6 = O ( n log n )
3.2 Hashing
Consider a hash table of size 7 with hash function h ( k ) = k mod 7. Draw
the table that results after inserting, in the given order, the following values:
19 , 26 , 13 , 48 , 17 for each of the scenarios below:

When collisions are handled by separate chaining.
When collisions are handled by linear probing.
When collisions are handled by double hashing using the secondary
hash function h ′( k ) = 5−( k mod 5)
