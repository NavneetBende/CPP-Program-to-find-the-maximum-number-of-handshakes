# CPP-Program-to-find-the-maximum-number-of-handshakes

Maximum Number of Handshakes in C++
Here we will discuss how to find the maximum number of handshakes which can happen between N number of people given the fact that any two people shake hands exactly once using C++ programming language.

Maximum number of handshakes
Approach :
For the number of handshakes to be maximum, every person should hand-shake with every other person in the room

i.e. all persons present should shake hands.

For the first person, there will be N-1 people to shake hands with
For second person, there will be N -1 people available but as he has already shaken hands with the first person, there will be N-1-1 = N-2 shake-hands
For third person, there will be N-1-1-1 = N-3, and So On…
Therefore the total number of handshake   =   ( N – 1 + N – 2 +….+ 1 + 0 )   =   ( (N-1) * N ) / 2.

Algorithm
For N = 8
handshakes  =  ( (N-1) * N ) / 2  =  ( 8 x 7 )/2  =  28
Print Result
Maximum number of handshakes in C++
While loop in C
Related Pages
Quadrants in which a given coordinate lies
 
Permutations in which n people can occupy r seats in a classroom
 
Addition of two fractions

Replace all 0’s with 1 in a given integer

Can a number be expressed as a sum of two prime numbers

C++ Code
Run
// C++ program to find the maximum number of handshakesM
#include<iostream>
using namespace std; 

int main()
{

    //fill the code
    int num = 9;

    int total = num * (num-1) / 2; // Combination nC2

    cout<<"For "<<num<<" people there will "<<total<<" handshakes";

    return 0;

}
Output
For 8 people there will be 28 handshakes
