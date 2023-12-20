## ARMssembly 0 

### Approach :

The main part of this code is func1 :




![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/19d6834f-3ace-4036-84af-ea153cefeba7)




The two inputs of cmp w1,w0 comparison are unsigned lower/below or same, which means that when is less than , go to this block. The return value under this branch is actually the larger number. Another branch returns a larger number in the same way.

Therefore, the function (func1) is to compare the two inputs and return the larger number. The larger number in the question is 3742084308(I tried putting in the smaller number once just to check ,the string it returned was not the flag, thus working of the function(func1) was clear to me), then a simple command ‘{:x}’.format(3742084308)( which converts strings to hex) gave the flag

![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/4a2d6f5e-7bf7-4b08-8d58-c938f4305e3b)

### FLAG :



picoCTF{df0bacd4}

