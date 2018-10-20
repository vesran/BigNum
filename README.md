# BigNum
BigNum is a Java class used for the computation of any positive integers, especially large numbers. 

# Usage
    New_BigNum(int)
    BigNum* New_BigNum_By_String(char* strSequence)
    
You can initiate a BigNum with an integer or a sequence of char (string).

    BigNum* number = New_BigNum(100);
    BigNum* number2 = BigNum* New_BigNum_By_String("4891456418913542");

# Methods
    struct BigNum* (*Add)(struct BigNum*, struct BigNum*)
Add returns the addition between two BigNum.
It returns NULL if at least one of the parameters is NULL.

    struct BigNum* (*Sub)(struct BigNum*, struct BigNum*)
Sub returns the subtraction between two BigNum,
the first minus the second in parameters.
It returns NULL if at least one of the parameters is NULL or the result is negative.

    struct BigNum* (*Mult)(struct BigNum*, struct BigNum*)
Mult returns the multiplication between two BigNum.
It returns NULL if at least one of the parameters is NULL.

    struct BigNum* (*Div)(struct BigNum*, struct BigNum*)
Add returns the division between two BigNum.
It returns NULL if at least one of the parameters is NULL or in case of a division by zero.

    struct BigNum* (*Power)(struct BigNum*, struct BigNum*)
Power returns the result of the first BigNum raises to the second BigNum power.
It returns NULL if one of the BigNum is NULL.

    struct BigNum* (*Factorial)(struct BigNum*)
Factorial returns factorial of a BigNum.
It returns NULL if the BigNUm is NULL.

    int (*Compare)(struct BigNum*, struct BigNum*)
To compare two BigNum and returns a positive int if the first BigNum is bigger than the second
a negative int if not and 0 if equals.

    void (*Free)(struct BigNum*)
To free the allocated memory for a BigNum.

    void (*View)(struct BigNum*)
To display the BigNum.

    BigNum* Combinaison(BigNum* k, BigNum* n)
It returns the combinaison nCk of two BigNum n and k.
