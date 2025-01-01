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

List of algorithms our interpreter is able to work on:
1. Sum of first N numbers

10 N = 10
20 SUM = 0
30 FOR I = 1 TO N STEP 1
40 SUM = SUM + I
50 NEXT I
60 PRINT SUM

2. Factorial of N

10 N = 5
20 FACT = 1
30 FOR I = 1 TO N STEP 1
40 FACT = FACT * I
50 NEXT I
60 PRINT FACT

3. GCD of Two numbers

10 A = 20
20 B = 15
30 A = ABS(A)
40 B = ABS(B)
50 WHILE B > 0
60   TEMP = B
70   B = A MOD B
80   A = TEMP
90 WEND
100 PRINT A

4. Reverse a number

10 N = 1234
20 REVERSED = 0
30 WHILE N > 9
40  DIGIT = N MOD 10
50  REVERSED = REVERSED * 10 + DIGIT
60  N = INT(N / 10)
70 WEND
80 REVERSED = REVERSED + N
90 PRINT REVERSED

5. Check if the number is prime

10 N = 101
20 IF N <= 1 THEN 
30   PRINT "The number is not a prime number."
40 END IF
50 IS_PRIME = 1
60 FOR I = 2 TO INT(N / 10)
70   R = N MOD I
80 IF R = 0 THEN 
90   IS_PRIME = 0
100 END IF
110 NEXT I
120 IF IS_PRIME = 1 THEN 
130   PRINT "The number is a prime number."
140 END IF
150 IF IS_PRIME = 0 THEN
160   PRINT "The number is not a prime number."
170 END IF

6. Check if a number is a palindrome

10 N = 456
20 ORIGINAL = N
30 REV = 0
40 WHILE N > 0
50   DIGIT = N MOD 10
60   REV = REV * 10 + DIGIT
70   N = INT(N / 10)
80 WEND
90 IF ORIGINAL = REV THEN 
100 PRINT "The number is a palindrome"
110 END IF
120 IF ORIGINAL <> REV THEN
130 PRINT "The number is not a palindrome"
140 END IF

7. Maximum digit of a number

10 N = 1273
20 IF N < 0 THEN
30   N = ABS(N)
40 END IF
50 MAXDIGIT = 0
60 WHILE N > 0
70   DIGIT = N MOD 10
80   IF DIGIT > MAXDIGIT THEN MAXDIGIT = DIGIT 
90  END IF
100   N = INT(N / 10)
110 WEND
120 PRINT MAXDIGIT

8. Sum of digits

10 N = 1234
20 IF N < 0 THEN
30   N = ABS(N)
40 END IF
50 SUM = 0
60 WHILE N > 0
70   DIGIT = N MOD 10
80   SUM = SUM + DIGIT
90   N = INT(N / 10)
100 WEND
110 PRINT SUM

9. Multiplication table

10 N = 5
20 FOR I = 1 TO 10 STEP 1
30 PRINT N * I
40 NEXT I

10. The Nth Fibonacci number

10 N = 10
20 IF N <= 0 THEN 
30   PRINT "Invalid input! Please enter a positive number greater than 0."
40 END IF
50 A = 0
60 B = 1
70 FOR I = 1 TO N - 1 STEP 1
80 TEMP = A + B
90 A = B
100 B = TEMP
110 NEXT I
120 PRINT A

