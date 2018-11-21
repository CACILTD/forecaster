## Solution


### Solution Hierarchy

At this point it is sensible to talk about the hierarchy of a solution.  Once a new solution has been defined or loaded, its structure can be seen in the Solution Explorer window.  A solution may contain one or more projects.  The projects can be related to one another, such as projects with the same dataset but with differing forecasting models, or they can be completely unrelated but grouped in the solution for convenience.  For example, all call volume forecasts in a contact centre could be grouped into one solution.  Figure 5 demonstrates that forecast projects for Motor, Home, Pet and Travel can be grouped in the same solution.

**[ IMAGE ]**

Each of these projects contains different sources of data, however, for the sake of simplicity it makes sense to group all of these forecasts in the same place.  For example, if other planners need to build forecasts in someone’s absence, all active forecast models will be in the same collection.
Notice in Figure 5 that within the Motor Sales forecast there are a number of sub-forecasts or project snapshots.  These snapshots represent a collection of Motor Sales forecasts that share common data with the project one level up.  The purpose of this hierarchy is to allow the user to keep a copy of all experiments considered valuable, for example a collection of forecast models that yield good predictions.


### Solution Management
The first part of the Solution group concerns itself with creating, saving and opening existing solutions.  Essentially, these are all the standard operations that a user would expect when creating, for example, a word document or similar.  More details follow in this section.
The second part of the Solution group focusses on the solution hierarchy and is covered in more detail in sections 0 and 0.

**[ IMAGE ]**

#### New Solution
The New Solution icon (or quick keys Ctrl+N) allows the user to create a new forecast solution.  
When the user selects to create a new solution, they are required to enter a solution name and, if necessary, change the location of the solution directory.  Once these parameters have been specified and the user presses the OK button, the new solution will be created.  

**[ IMAGE ]** 
Figure 7 Generating a New Solution

The application will then look similar to Figure 8, ready to accept data.  More details on this are covered in section 0.

**[ IMAGE ]** 
Figure 8 New Solution



#### Open, Close and Save a Solution
These are all standard windows processes, which operate in the same way as any windows application.
*	To open a solution, click on the Open icon, select the file of interest and select OK.  Alternatively press the Ctrl+O keys to access the same open solution dialog
*	To close a solution, click on the Close icon.  If the solution has had some changes before the last save, then the application will ask you if you wish to save the changes
*	To save a solution, select the Save icon.  This will then display two save options:
    -	Save:  Saves the solution under the current name.  Files can be saved directly by pressing the Ctrl+S keys
    -	Save As: This enables you to save the solution under a new name or in a different location

Additionally all of the above functionality can be executed from any point in the application using the quick access toolbar, displayed in the top left of the CACI Forecaster. 
 

**[ IMAGE ]**
Figure 9 Quick Access Toolbar


When a solution is saved, a solution directory is created and a number of files are placed in this directory.  If you wish to move a forecast solution without using Save As, for example if you have multiple solutions to move, you need to copy all elements in the solution directory to the new location, otherwise the hierarchy defined in the solution view will be broken.


#### Deleting a Solution
To delete a solution, delete the solution directory through the usual Windows Explorer or equivalent.


#### Recent Solutions
Links to recent solutions are available via the Home – Solution ribbon or in the main window in Home.  As checks are made prior to a solution appearing in the list, all recent solutions listed will be valid and accessible.  If files are subsequently deleted, they will not be displayed in the options list.
Selecting from this list will save you time and effort trying to find the location of previous solutions you may have been working on.






