# CoOp-Database
CoOp Database created using Python2.7, SQLite3, and Tkinter. The repo is missing files `coop.SQL` which is the SQL database that contains all of the CoOp info and `Coop.xlsx` which holds some director, goal, and department information. Both of these files have been withheld to protect personal information. The file `semesters.txt` is used to determine which coops are active.

The database enables a user to add/edit/delete coops, view coop trends by major, school, recruitment method, rotation worked, department, manager, director, see department staffing projections, and more. 

I used `py2exe` to create a standalone executable to distribute to others.

## Screenshots

<img src="https://github.com/alexkenan/CoOp-Database/blob/master/screenshots/7.png?raw=true" width="603" height="507" border="1" style="border:5px solid black">

This is the database homepage. It has some directions (more are in an attached doc file) and the user interacts with the database via the toolbar at the top. 

<img src="https://github.com/alexkenan/CoOp-Database/blob/master/screenshots/2.png?raw=true" width="603" height="507" style="border:5px solid black">

This is the page to add a CoOp to the database. The fields that contain text have been auto-filled by the program. The `Example` and `Help` buttons assist the user with correct formatting and syntax. There are similar pages for Find, Edit, and Delete.


![Major](https://github.com/alexkenan/CoOp-Database/blob/master/screenshots/3.png?raw=true)

This is one of the sorting pages, and shows the results of hitting the `Submit` button and hitting the `Submit - Verbose` button. The `Submit` button shows the name, department, and department description while the `Verbose` submit button shows name, major, college, rotation, recruitment method, station, manager, director, salary, and date the entry was inputted. Names have been removed.

![Export](https://github.com/alexkenan/CoOp-Database/blob/master/screenshots/4.png?raw=true)

This shows some export options for the database. `Export database` will export the entire database to a txt or xls file, `Export Semester CoOps` will export a specified semester's CoOps, and `Export Active CoOps` figures out which coops have completed 1-3 rotations and exports their data.

![Manager](https://github.com/alexkenan/CoOp-Database/blob/master/screenshots/5.png?raw=true)

Some options for managers - the most important was the six semester projection which shows which departments still needed to find coops for which upcoming semesters.

![Smart](https://github.com/alexkenan/CoOp-Database/blob/master/screenshots/6.png?raw=true)

Database dynamically detects when a new semester has started and tries to add the last one to the list of past semesters to re-figure out which coops are active.


##Ideas for Improvement
My next round of improvements would be to eliminate the need for `Coop.xlsx` and `semesters.txt` by bundling them all into `coop.SQL` as other SQL tables.

##Known Issues
I tried to write an auto-backup feature into the program, but experienced a mysterious `WindowsError` that I could not troubleshoot.
