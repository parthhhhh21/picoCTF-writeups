## new caesar 

### Approach :


Decided to write code to make the program run in reverse.

Stored the value in the question variable enc and as the key
could have been any character from a to p, I decided to
create a list named b16 so, that I can convert the encryption
for all possible keys. 


Reversing the function shift :
 
![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/a8fadb31-279d-453e-91d8-b8c760e6d9bd)







I looped through each value of enc and converted it for each possible key. We know that the index of i in ALPHABET needs to equal the character we are looking - 97 and the key -97 modulus 16.

![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/66408cbf-ff16-43d8-9ab1-b4ce5c987c92)


### FLAG :



picoCTF{et_tu?_1ac5f3d7920a85610afeb2572831daa8}






