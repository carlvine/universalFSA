This program defines the validity of input given a formal language definition of a Finite State Automaton. It utilizes multidimensional arrays to store the “state table” diagram of legal transitions, as well unordered_maps and sets to map any alphabetic symbol to their corresponding state.


Input must match the following structure:
# of final states
final states
alphabet 
transitions


Example:
	The following Finite State Automaton accepts strings of 1's and 0's with an odd number of 1's.

2                   //states
1					//final state
0 1					//alphabet
(0,0,0)				//transitions
(0,1,1)
(1,0,1)
(1,1,0)



Compilation:  Place both uniFSA.cpp and input.txt in
the current folder. From command line, compile and run uniFSA.cpp
through the following command:

	g++ uniFSA.cpp -std=gnu++0

*the last part was required with my GNU/gcc compiler in order to 
process <unordered_maps>. It may not be neccessary.

NOTE: Output is written to file outputFSA.txt
