**S3 Datastructures Lab\
Experiment 7**
-----------------------------------------------------------------

Question:
Implementation of Stack and Multiple stacks using one dimensional array in c

Solution:
Representation of a Polynomial:  A polynomial is an expression that contains more than two terms.  A term is made up of coefficient and exponent.  An example of polynomial is

P(x) = 4x3+6x2+7x+9

A polynomial thus may be represented using arrays or linked lists.  Array representation assumes that the exponents of the given expression are arranged from 0 to the highest value (degree), which is represented by the subscript of the array beginning with 0.  The coefficients of the respective exponent are placed at an appropriate index in the arrays.
A polynomial may also be represented using a linked list.  A structure may be defined such that it contains two parts- one is the coefficient and second is the corresponding exponent.  The structure definition may be given as shown below:

            struct polynomial
{
int coefficient;
int exponent;
struct polynomial *next;
};


Refer to the program!

--------------------------------------------------------------------

