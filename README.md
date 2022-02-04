# awn
calculates absolute winding number to describe trajectory during spatial navigation 
We calculate the absolute winding number to describe trajectory during spatial navigation
Didong Li, Andrei Niculescu, Alex Badea 02/04/2022

Content:

1. extract_data is for calculating the AWN of all files in one given folder

2. filerenamer 

3. AbsWinding.m is for calculating AWN from a n*3 data matrix, n is the number of files/experiments. Col-1 = time, col -2 = x-coordinates, col-3 = y-coordinates

SOP
1) Open MWM AnyMaze experiment for corresponding cohort
2) Open the File tab and click Export
3) Select Export Test Data and save in /alex/APOE_Behavior/MWM/Winding/######_Positions
4) Make sure each test file has the cohort date in the name

Calculating
1) Open filerenamer.sh within XCode or another editor
2) Update the pathways and file/folder names in the code
3) Use the command terminal to run the file to change the test file names to include the mouse id, day, and trial. If using iTerm, the command is sh filerenamer.sh
4) Now that the files are renamed, open AbsWinding.m within MATLAB. Make sure that both AbsWinding.m and extract_data.m are next to the test data folder.
5) Change the pathways and file/folder names within the code and run the script.
6) Now that you have a csv file with the winding numbers, add them into the concatenated MWM Data Sheet: APOE_MWM.xlsx''

Good luck!
