During the fall semester of 2020, I and 7 other students taking the course CSC207H1 F - Software Design at the University of Toronto were required to 
make a Conference program. This was done in 3 phases:

<h4>Phase 0</h4>
Independently create CRC cards for the Phase 1 outline of the project.

<h4>Phase 1</h4>
Collaborate with your group to create a program satisfying the Phase 1 outline.

<h4>Phase 2</h4>
Implement additional mandatory extensions and a minimum of 4 other new features from a list of optional extensions.

<h3>Feedback</h3>

1. Your project makes good use of:
* Good use of Single Responsibility Principle, class separation are logical and clean
* A gateway class that connects database so other classes don't need to interactive with storage directly and it is easier to add other means of storage.
* Good use of Dependency Injection
* Since you store all of your users in the same location, having one UserFactory makes sense. Good job!
2. Someone using your program will see:
* Text based interface, much improved then phase 1. There are some UX issues such as inconsistency in commands and some minor bugs.
* An event system with many additional features such as multiple speakers event, VIP attendee, statistics, etc
* Improved user with more information
* A good messaging system similar to a email client.
3. Good next Steps include:
* Few more design patterns can be applied, such as using Facade to simplify controller & presenter interfaces. This will increase encapsulation and extensibility respectively.
* Consider storing your presenter strings as instance variables at the top of the class. This will make it easier to find and change them if necessary. Hard-coding values into each method makes any changes more time consuming.
* You made a good start with helper methods. It would be a good idea to continue the process of looking for blocks of code that work together to do something specific and extracting that block into a new helper method. This might simplify some of your longer methods.
* For larger switch statements and larger classes (see UserController, OrganizerController, etc.) can you think of a way to refactor so that it would be easier to add new functionality to your program in the future without reading through so many lines of code?
* Is there a big difference between a Talk, a Party, and a Panel? Often program specifications are written by people who know how they want to use the program but not necessarily how to program. It is up to you to decide whether or not you need separate classes for different event types or whether you can just store a list of speakers and add to it when necessary. In the latter design, it would be easy to turn one type of event into another, if required.
* Add a graphical UI or improve the user experience on the text interface (i.e shortcuts, key prompts, easier navigation, see other command line programs).

