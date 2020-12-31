# Learnt_from_Universities
Diverse fields of knowledge related to CS learnt from universities.

## Self_made_Tools
   1. detectInputType method
      - Detect input type and continuously requesting users until the correct type (integer) is given.
      - A detection of String "STOP" is included to exit the execution.
      - Returns a String instead of integer so as to fits with the detection of String "STOP".
      - The conversion of String to integer, as well as the stop of execution, relies on the main method (and the if-else statement inside).
      - The input of the method detectInput(String detectTarget) also request the user's input to be in a string form, though the user never knows.

## Achievements_Earned
   1. detectPrimeNumber
      - One of the exercise I did when I started to learn programming.
      - Aims to find the biggest prime number between 1 and the user's input.
      - Definition of prime number is that it can only be divisible by 1 and itself.
         - If the number(n) is divisible by other integers(i), it is not a prime number.
         - `n % i == 0`, n is not a prime number.
      - If the (Divisor) > (Dividend)/2, there must be a remainder when testNumber modulus testTool.
   2. printoutDiamondWith3LoopsSimpleVersion
      - A classwork requires us to print out a diamond shape in 3 for loops.
      - The initial version that I finished the task, with the Math.abs() method used as the task recommended.
      - "Divide and conquer" method is used to seperate the diamond into two parts.
      - The equations found is more based on listing out cases and finding the common factors.
   3. printOutDiamondWith3LoopsAdvancedVersion
      - An upgrade version of the classwork, though the max. no. of lines is inserted by the user.
      - Better structures using multiple "if-else" statements and mathematical calculations.
      - "Divide and conquer" method is also used as the above one.
      - The program view the no. of spaces and stars as a whole first, and then print out both of them seperately.
