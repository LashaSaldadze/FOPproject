# FOPproject: Java interpreter for BASIC programming language
This is a group project for KIU CS course, second midterm
Team members:
Lasha Saldadze (Roles: group leader, writing and testing with BASIC language's algorithms, writing cleanedCode(), parseAndExecute() and evaluateCondition() methods)
Mariam Salukvadze (Roles: writing handleIf() and handleNext() methods)
Nikoloz Kurtsikidze (Roles: writing handleWhile() and handleFor methods)
Nikolozi Katamadze (Roles: writing handleAssignment() and handleInput() methods)

Language subset:
Our interpreter supports: variable assignment, arithmetic operations (+, -, *, /, %), conditional statements (if, else), iterative control flow (while or for loops).

Instructions:
Upon running the program, user will be greeted with the message "Enter BASIC code line by line. Type \"FINISH\" in a new line to finish:". After inputing the (valid) BASIC code in the console, the interpreter will look over and analyze it line by line, after which it will output the algorithm result. If the code inputed was invalid, the interpreter will be able to return correct error messages to the user. 
