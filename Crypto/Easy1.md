## Easy1

### Approach :

Downloaded the file given in the question :

![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/9140aa95-5c08-47dd-8609-e5c29b9795bb)

For each letter in the key:
Find the row corresponding the the letter

In the row, find the column which contains the matching ciphertext letter

The matching plaintext letter is noted at the top of the column

For example, S and U combine to give C( C is in the same row as U )

### FLAG :

picoCTF{CRYPTOISFUN}
