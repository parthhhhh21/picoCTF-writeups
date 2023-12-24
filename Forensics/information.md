## information

### Approach :

Downloaded the image from the web using the 'wget' command :


![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/d2d36d2e-f7c8-44e6-abe0-e44ff97679f8)


Learnt about a new command "exiftool" which is used for reading, writing, and manipulating image, audio, video, and PDF metadata :


![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/3b3f6943-5c7e-4da4-915a-eeb8a191b105)


Here, we see a text against "License" which is encoded. So, copied that text which seemed to be base64 encoded and converted to ASCII :


![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/f024cdfb-ad34-44cc-950f-cd38ae8f4853)

Found the flag.

### FLAG :

picoCTF{the_m3tadata_1s_modified}


