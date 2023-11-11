MOD1


Created a first list called message with the text from the question(message.txt)


A second list called decryptGuide with the orientations to decode the result :
•	Alphabet: 0-25 is the alphabet in uppercase using the lib string
•	Decimals: 26-35 are the decimal digits
•	Underscore: 36 is an underscore


Finally, a for loop which will get every number of the message and run it in the euclidean function with the modulous 37 provided by the challenge and turn into a decrypted number, after that, get the current number as an index in the decryptGuide to get the result in the print at the end.


![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/8d7ce85c-bb23-4838-8476-b183688f0cbc)


 

FLAG :



picoCTF{R0UND_N_R0UND_ADD17EC2}



