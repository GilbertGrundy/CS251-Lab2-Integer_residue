Gilbert Grundy CS251
Lab #2

Program is a simple, one file program, which calculates the residue of
numbers in the form of: a^k mod n.

Given these values by the command line, the program prints a sequence
of values corresponding to: a^(2^k) mod n.

The program stops once it has the required values to do the calculation,
and highlights which values are required for the calculation. The user can 
re-run the calculation before leaving.

Sample Program Run:

* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *

Please enter a vlaue for a: 17
Please enter a value for k: 13
Please enter a value for n: 123

17^(2^0) MOD 123 = 17*
17^(2^1) MOD 123 = 43
17^(2^2) MOD 123 = 4*
17^(2^3) MOD 123 = 16*


17^13 MOD 123 = 104

Would you like to run the program again? y/n: y


Please enter a vlaue for a: 22
Please enter a value for k: 16
Please enter a value for n: 88

22^(2^0) MOD 88 = 22
22^(2^1) MOD 88 = 44
22^(2^2) MOD 88 = 0
22^(2^3) MOD 88 = 0
22^(2^4) MOD 88 = 0*


22^16 MOD 88 = 0

Would you like to run the program again? y/n: n

* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *

So:

17^13 MOD 123 = {(17^1 MOD 123)*(17^4 MOD 123)*(17^8 MOD 123)} MOD 123
              = {17*4*16} MOD 123
              = 1088 MOD 123
              = 104
              
2nd Example is a little less interesting:

22^16 MOD 88 = 22^16 MOD 88
             = 0 MOD 88
             = 0
