# heartTransplant
Assignment from CS11 Course 


A heart transplant is a surgical procedure that replaces the person’s heart with a donor heart. A person may require a heart transplant for several reasons including congenital, arterial and muscle diseases or for unforeseen reasons such as accidents or viral infections.

The donor heart is matched to the recipient by blood type. Additional variables are also used to decide which recipient receives a heart if there are not enough hearts available for all recipients waiting for a transplant. The variables included in the decision may include the recipient state of health, cause of the heart condition and the urgency of the transplant.

The primary goal of this project is for you to write a HeartTransplant class that has the ability to select the patient, from a pool of patients, with the highest potential to survive the longest after the heart transplant surgery. Used the HeartTransplantDriver to test the methods within the HeartTransplant class.

Files Provided
HeartTransplantDriver.java
This is the program you should compile and run.
It builds a HeartTransplant object and calls instance methods on it.
No need to make changes to it, but you are welcome to change it if you want. It is for testing purposes only.
SurvivabilityByAge.java
Stores information about the survivability of patients, by age, after n years post heart transplant surgery.
SurvivabilityByCause.java
Stores information about the survivability of patients, by heart condition cause, after n years post heart transplant surgery.
Patient.java
Stores patient information.
Contain constants representing patient codes (health condition code, gender code, urgency code, ethnicity code…)
Data.txt
Contains patient information, as well as survivability by age and cause rates.
This file should be piped when executing HeartTransplantDriver
How to run the driver: 
Compile: javac HeartTransplantDriver.java
Execute: java HeartTransplantDriver < data.txt
HeartTransplant.java
This is the file you will write your code on.
Provided as an empty file, complete it based on documentation.
Understanding the Driver:
The HeartTransplantDriver will create an HeartTransplant object using its default constructor. 
The driver will then initialize the three instance variables in the object using the following instance methods:
readPatients(int numberOfLines)
readSurvivabilityByAge(int numberOfLines) 
readSurvivabilityByCause(int numberOfLines)
Finally, the driver will test the three instance methods on the object:
getPatientsWithAgeAbove(int age)
getPatientsByUrgency( int urgency)
getPatientForTransplant()

Data File and Execution
We provide a data file with real data that is the input for the program. The data file contains information on 21 people of the same blood type, 24 survivability by age rates, and 15 survivability by heart condition cause rates. More on the data file format below.

Compile the program as follows:

javac HeartTransplantDriver
Execute the program as follows:

java HeartTransplantDriver < data.txt
The file data.txt is redirected as the input for the program HeartTransplantDriver and can be read using the StdIn library functions StdIn.readInt() and StdIn.readDouble().

Data File Format
The data file is divided in three sections. The first section is the person section, the second the rates of survivability by age section, and the third is the rates of survivability by heart condition cause section.

First section: person

The first line of this section has an integer that refers to the number of persons in the file. The file has one person per line in the following format:
PersonID Ethinicity Gender Age Cause Urgency StateOfHealth
 
The example below has 3 persons, the first person’s ID  4101, Ethnicity 10, Gender 13, Age 75, Cause 3, Urgency 8, and StateOfHealth 7. You can see the meaning of each code in the Person.java file.
Second section: survivability by age

The first line of this section has an integer that refers to the number of survivability by age rates in the file. The file has one rate per line in the following format:
Age YearsPostTransplant Rate
 
The example below has 8 rates, the first rate specifies that people with age LESS than 1 year old, 5 years post transplant have a survivability rate of 83.6%.
Third section: survivability by heart condition cause

The first line of this section has an integer that refers to the number of survivability by cause rates in the file. The file has one rate per line in the following format:
Cause YearsPostTransplant Rate
 
The example below has 5 rates, the first rate specifies that people with heart condition cause 4 (heart muscle disease), 1 year post transplant have a survivability rate of 89.4%.You can see the meaning of each code in the Person.java file.
3
4101  10  13  75  3  8  7
4102  11  14  78  4  9  5
4103  12  14  40  3  8  5
8
 1  5 83.6
 6  5 87.4
 11 5 86.8
 18 5 90
 35 5 86.9
 50 5 88.8
 65 5 87.8
120 5 84.3
5
4 1 89.4
1 1 82.1
3 1 87.1
0 1 88.2
2 1 88.2

If viewing this assignment, please follow Rutgers University Honor Code 
