# LL-1_Parser
LL-1 Parser implemented completely in C++ (without Lex/YACC)
Compiler Design Project:

Compiler Design Project:


	***LL(1) Parser Implementation***

	--> Objective: To implement a LL(1) parser which can parse a given stream of tokens according to a given LL(1) grammar.

	--> Languages and tools used: C, C++.

	--> Input: The LL(1) parser will read following two things as input from two different input files.
		
		(i) Given LL(1) grammar according to which the parser will work.
		    It must be in the following format.

			_______________________________________________________________
		       |                                                               |
		       | (a) Each production should be written separately.	       |
		       |     For eg. A -> B | Cb     is invalid.		       |
		       |     It should be written as:				       |
		       |		A -> B					       |
		       |	        A -> Cb					       |
		       | (b) Each non-terminal should be written as  capital   	       |
		       |     alphabets.						       |
		       | (c) Each terminal symbol should be written as small alphabets.|
		       | (d) The given grammar must be non-ambiguous and should adhere |
		       |     by the rules of LL(1) grammar.		               |
		       | (e) It should be present in a separate file named grammar.txt |
		       |     in the same directory where parser is present.	       |
		       |_______________________________________________________________|

		(ii) Given the stream of tokens, which the parser will parse according to above grammar.
		     It must be in the following format.

			_______________________________________________________________
		       |                                                               |
		       | (a) Each token should be present separately with a single     |
		       |     white-space between them.				       |
		       |     For eg. let a,b,c,d are 4 tokens, then the file can be:   |
 		       |	a b c d        or      c b d d a b     etc.            |
		       | (b) It must be present in a separate file named string.txt in |
		       |     the same directory where parser is present.	       |
		       |_______________________________________________________________|

	--> Execution instruction:
		
		The LL(1) parser will be present inside a file named "parser.cpp".
		It must be compiled before executing.

		Compile command:
			_______________________________________________________________
		       |							       |
		       |           	   g++ parser.cpp -o parser	       	       |
		       |_______________________________________________________________|

		Execute command:
			_______________________________________________________________
		       |							       |
		       |           	        ./parser              	       	       |
		       |_______________________________________________________________|

	--> Output:

		Output will be generated every time the program is executed.
		Output will be displayed on screen as well as it will get autosaved inside a separate file named "ouput.txt" for every attempt of execution.

		Output will be shown in following format:

			________________________________________________________________
		       |                                                                |
		       | Case 1: If any of the input file is absent it will simply      |
		       |         print an error message and terminate.                  |
		       | Case 2: If the tokens present inside the "string.txt" file is  |
		       |         not identified by the grammar then parsing will fail   |
		       |         and it will display error message with sufficient info.|
		       | Case 3: If the string is successfully parsed by the parser     |
		       |         according to the grammar, then it will print success   |
		       |         with sufficient information about parsing process.     |
		       | 							        |
		       | NOTE: Parsing table will be displayed for each execution,      |
		       |       however the construction process of parsing table 	|
		       |       involving FIRST() and FOLLOW() sets shall remain 	|
		       |       abstracted.						|
		       |________________________________________________________________|

	--> Submitted to: Sir Dinesh Gopalani

	--> Submitted by: UJESH MAURYA (2015UCP1338)
			  HITESH YADAV (2015UCP1520)



