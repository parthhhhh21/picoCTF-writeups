## basic-mod2

### Approach :

THe file given in the question :

![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/e5f11013-0e44-4d47-99c7-bebec0f8cc51)

Firstly, I needed to find the remainder of each element when divided by 41 so, wrote a simple code in order to do the same :

![Screenshot 2023-12-31 161914](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/48ddaa12-1bf6-4252-9b5e-859f2fccc556)

Secondly, I needed to find the modular inverse of each number in the list so, used bard.ai to get the same : 

![Screenshot 2023-12-31 162030](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/e6eccd89-79d6-4707-bbd0-f62cfa90f966)

Finally, according to the instructions given in the question :


•	Alphabet: 1-26 is the alphabet in uppercase using the lib string

•	Decimals: 27-36 are the decimal digits

•	Underscore: 37 is an underscore

I did this manually :

![Screenshot 2023-12-31 162931](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/a7f87c6a-ec2c-48a4-9e77-1f31b7fa6b1a)


### FLAG :

picoCTF{1NV3R53LY_H4RD_DADAACAA}
