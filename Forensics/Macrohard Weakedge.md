## Macrohard Weakedge
### Approach :

connected via wget https://mercury.picoctf.net/static/2e739f9e0dc9f4c1556ea6b033c3ec8e/Forensics%20is%20fun.pptm : 

![Screenshot 2023-12-20 193500](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/62845936-996f-42f5-bcfa-362f59ee125a)

used file ./Forensics\ is\ fun.pptm to see what it reeally is :

![Screenshot 2023-12-20 193507](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/fb47532d-8d09-44d2-b197-b65cb5865709)

it contained some .pptm file which i later learnt is a ppt file Macro-Enabled,a feature which let you write code to automate tasks.
learnt that the ppt or pptm file is able to be decompressed by changing the extension to .zip and use tools to unzip the file.
so, used unzip ./Forensics\ is\ fun.pptm. it displayed a bunch of files :

![Screenshot 2023-12-20 193518](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/3f0b5afe-89d3-400b-a095-9322f7498cc1)

![Screenshot 2023-12-20 193529](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/3f15a345-7da2-47c8-bee9-3f8ff9b68d1d)




but, got lucky when i thought that the flag was hidden in some file named "/ppt/slideMasters/hidden" (tried this first because it was obvious) 
so, used cat ./ppt/slideMasters/hidden and got a message : 

![Screenshot 2023-12-20 193545](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/78bdb391-d3d9-4ccd-a538-1276fe8776da)


which had to be converted from base64 to ascii which gave the flag :


![Screenshot 2023-12-20 194422](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/c273aefd-14c3-4db2-8d00-bb427af2aaab)

### FLAG : 


picoCTF{D1d_u_kn0w_ppts_r_z1p5}

