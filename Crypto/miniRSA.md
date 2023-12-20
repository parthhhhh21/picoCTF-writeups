## miniRSA

### Approach :

 The modulus N is far too large to factor. However, there is a caveat. c = pow(m,e,n). 
 However, what if m ^ e < n? Then the modulus never comes into play, and c = m ^ e. Not only that, but e in this case is very small: 3.
 We can clearly see that c is much smaller than n, meaning that it might just be possible that m ^ e < n. If that is the case, we can just take the cube root of c to find m (m ^ 3 = c so c = m ^ (1/3)).

 ![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/45732edd-256f-4447-b15e-b72a4127de9b)


These numbers are very large, so we need to make sure that our cube root is precise enough to list every digit.

![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/338718dd-0bc4-40ec-8572-301999c8975e)

and got this :


![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/78e9337e-78cb-41ce-bebe-a74adf264bea)



this is a hex and thus, can be converted to ASCII and we get the flag.



![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/866ade4b-dff5-4c96-b8f3-5ac36583efce)



### FLAG :

picoCTF{n33d_a_lArg3r_e_d0cd6eae}







