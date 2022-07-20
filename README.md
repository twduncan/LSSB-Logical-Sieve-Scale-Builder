# LSSB-Logical-Sieve-Scale-Builder
Logical sieves define octave-repeating scales according to basic applications of number theory. These rudimentary command line programs help to simplify the numeric tasks necessary to translate a scale into a set of sieve parameters or vice versa. The theory behind this concept is explained in detail in the paper *Scale Generation with Logical Sieves*. **ScaleToSieve** analyzes an octave-repeating scale and emits an 8-digit encoding specific to that scale. **SieveToScale** will translate an 8-digit encoding to a distinct octave-repeating scale.

# Installation
These two short programs are intended for commandline execution. After cloning the repository, run the following two lines to build the programs:

`g++ -o scaleToSieve scaleToSieve.cpp scale2sieve.cpp`

and   

`gcc -o sieveToScale sieveToScale.c scale.c`.

Test the programs with these two lines:   

`$./sieveToScale 15 48 0 0 1 0 2 1 2 0`   
`$ 48 50 52 53 55 57 59 60 62 64 65 67 69 71 72`   

and   

`$ ./scaleToSieve 60 62 64 65 67 69 71`   
`$ 0 0 1 0 2 1 2 0`.   
