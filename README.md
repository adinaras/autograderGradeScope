# AUTOGRADER for GRADESCOPE using diff
## Description:
### Uses diff command to compare expected output with student's submission output

## Steps for setup:
1. Preffered start would be to have the solution to the project
 - Redirected input for the projects is assumed - Example: when run from command line: ./a.out < input1.txt
 - input1.txt consists of the input to the program
2. These test cases are your input files that are stored in the /tests folder
 - Come up with as many test cases as you may want
 - These are to be saved in the format - input1.txt, input2.txt...
3. For each of the specific test cases, generate the corresponding output files
 - These are to be saved in the format - output1.txt, output2.txt...
 - These are the expected output files to be tested against
 - Stored in the /tests folder
4. makefile: 
 - This is the script that compiles the uploaded cpp file and generates the executable file (exe)
 - The students MUST upload their submissions with the name 'project_test.cpp'
5. test.bats:
 - You see test cases starting with @test
 - diff_files() is a function where the comparison happens
 - Various options for the diff command can be added here
 - For more info please do 'man diff'
 - compiletest: tests if program compiles
 - test1/2/3: 
    - runs the exe with redirected input file and stores temperory ouput in testOutput.txt
    - run diff_files calls the diff_files() function with the two parameters (student's output and the expected output)
    - If the outputs do not match, the for loop prints the comparison with the mismatched lines
 - testclean: makes sure the exe gets cleaned properly
6. weights.txt: This file holds the breakdown of points for each test case
7. run_autograder:
 - No changes here
 - This is the master shell script file that runs everything
8. requirements.txt and setup.sh:
 - No changes here
9. autograder.py:
 - main python file that grades and assigns points to give it to GradeScope for displaying
10. The solution program need not be uploaded

## Steps to configuring GradeScope:
1. Go to your course's assignments page
2. Click on 'Create Assignment' and select 'Programming Assignment'
3. Fill out the information in the next page and create the assignment
4. Once created, in the 'Configure AutoGrader' tab on the left:
 - Upload a zip file of all the files from the setup 
 - The files need to be zipped directly and should not be one level deep inside a folder
5. After uploading, click on 'Update Autograder'
 - This might take a couple of mins

You can test the autograder by uploading your solution.



## Acknowlegments: 
Aditya Narasimhan
Gregory Madra
Sanjana Mudduluru
Sudhindra Gopal Krishna
Monique Shotande

Copyright © 2022 adinaras
