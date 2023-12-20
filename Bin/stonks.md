Stonks :


Connected to nc mercury.picoctf.net 16439 and got the following :


![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/cbe3c57b-d297-4e4c-aab8-a658827145b5)

Chose the first option, it asked about ‘API token’. I tried to view memory as hex bytes and see if I spot anything. The output I got was some hexadecimal, that was probably ASCII. 

![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/24da4026-ee65-4dff-964a-0c9ced6988af)

Converted hexadecimal to ASCII :

![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/5121f247-c986-47d6-ab66-8282182a9eb1)

As you can see ,the string  'ocip{FTC0l_I4_t5m_ll0m_y_y3nbc7ceac6ÿ»}' needs to be formatted. So, I wrote a code in which it reverses the character one by one at an interval of 4( as you can see)  and got the flag:

![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/e22428e6-70b1-4570-bb2b-d8b6eedd3c4e)


FLAG :


picoCTF{I_l05t_4ll_my_m0n3y_c7cb6cae}






