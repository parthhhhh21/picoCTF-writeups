GDB Babystep 1 :


First, let’s open the downloaded file ‘debugger0_a’ :

![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/804ae262-dacc-40de-a7cb-34cad7a2e97d)

To get an overview of functions ,  I passed a command- info functions :

![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/2cf03bb4-0705-4c4e-a264-12eb7d727aad)

Our prime target here, is the main function , thus the command ‘disas main’ gives the contents of the main function :

![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/32f5a263-ea22-490a-92fb-3762622d7003)


As given in the question, the flag is in the eax register , which is “0x86342”. Thus, converting this hexadecimal to decimal would give the flag.


![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/a505392d-24cd-43e3-ac79-e142b3aac228)

FLAG :


picoCTF{549698}



