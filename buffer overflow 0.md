Buffer overflow 0:



The one thing that I noticed is that we are printing the flag on a segmentation fault, which is an error. If the flag printf() resides within sigsegv_handler(), then we can safely assume that we must figure out how to trigger a segmentation fault.


![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/a11e4571-4c67-42b0-9a53-c4ab56f8ca5e)

We see that on line 40, the horrible gets() is called, and reads buf1 (the user input) onto the stack. The user can simply overflow this length, and the program will pass their input into the vuln() function to trigger a segmentation fault:

![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/a91cf9fa-60e2-405d-8d90-666f980e6367)


On segmentation fault :


![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/5dded3eb-6958-4cc0-846b-c6a5365a2871)

We get the flag!

FLAG :



picoCTF{ov3rfl0ws_ar3nt_that_bad_9f2364bc}


