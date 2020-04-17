# fizzBuzzSolution
Solution to the fizzBuzz Problem, where input is a JSON file and need to be varified as valid FizzBuzz String.

/**
* update file extensions and remove sufix .tmp for executables.
*/

Attached are two executables and the running project archive named follwoing

	fizzBuzzSolution-0.0.1-SNAPSHOT-jar-with-dependencies.jar is independent and has dependencies included inside the jar file.
	fizzBuzzSolution-0.0.1-SNAPSHOT.jar 
	dshukla.fizzBuzzSolution.jar

How to use these files - 
	To import the project source code, one can import the following project to some IDE and run it
	To test executable one can use following command
		java -jar fizzBuzzSolution-0.0.1-SNAPSHOT-jar-with-dependencies.jar  C:\resources\SampleJSON_valid.json


Dependendies used 
Maven => as build tool
Junit5 for testing => come with jupiter engine and jupiter api
json-simple => for JSON manipulation

Approach used - 
	1. Spent most of time on test case and Designing.
	2. TestCases - Have written around 20 test cases
			a. Written an automated utility(FizzBuzzJSON_Test) to ceate random JSON input file to test the logic
			b. Was trying to use more new features like repeat and nested from Junit5
			c. Code design has been keeping SOLID principles in mind, 
				I. FileInputOutputHandler is responsible for parsing input and output console.
				II. FizzBuzzValidator is responsible for managing the request, processing it and giving result on demand.
			d. Test cases has been moduled into few category 
				I. AutomatedTest_NegativeCase_FizzBuzzValidationLogicTest & AutomatedTest_PositiveCase_FizzBuzzValidationLogicTest for automated test cases
				II. Invalid parameter test cases has been added.
				III. A list of invalid file test cases has been added.
