# DNA and RA Decode Sequence 

Dioxyribonucleic Acid (DNA) and Ribonucliec Acidare long molecules forming the genetics and is copied over the generations. 
One of the components of DNA/RNA is a nucleotide which has nucleobases:
1. Cytosine (C) 2. Guanine (G) 3. Adenine (A) 4. Thymine (T) [Occurs in DNA only instead of Uracil(U)] 5. Uracil (U) [Occurs in RNA only instead of Thymine(T)]
Combination of these nucleobases form a DNA/RNA. Consider this table for solving theproblem below:

Neucleobase > Binary Value ----- C > 001  G > 010  A > 011  T > 101  U > 110  

Additionally, the sequence 000 is used to identifyDNA and 111 identifies RNA.

Given a sequence of binary integers of 3-bits each, you are expected to decode it in the readable format and also correct any errors in the input sequence.
   
Consider an example of an input as:000001001011101010010110011
Now, the first 3 bits of the input are 000 which depicts that the remaining set of binary digits should be interpreted as DNA sequence. 
Now, we group the remaining bits into a set of 3-bits which can be represented as 001 001 011 101 010010 110 011. 
Upon decoding this, we get the sequence as CCATGGUA. Now, since the letter U is an invalid nucleobase in a DNA, it should be replaced with T. 
Therefore, after correcting the output, the final output should be: - CCATGGTA

Sample Input For Custom Testing 000001001011101010010110011 
Sample Output CCATGGTA 
ExplanationFrom the input, we can identify that the first 3 digits are 000 which represents a DNA sequence.
That also means that if the input contains U (Uracil) in the sequence it should be replaced with T (Thymine). Upon decoding the sequence, we get CCATGGUA as the output. Since this is a DNA sequence, all fhe occurrences of U would be replaced by T. 
Therefore, the above output.

Sample Case 1 
Sample Input For Custom Testing 111001001011101010010110011 
Sample Output CCAUGGUA 
ExplanationThe first 3 digits of the input indicate that the input is a RNA sequence. Upon decoding, we would get the above output.




