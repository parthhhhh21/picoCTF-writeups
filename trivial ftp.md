trivial ftp 


downloaded wireshark to see the files : 


![Screenshot 2023-12-20 190043](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/8a39532b-d98a-473a-b03e-39659e6da28d)

learnt how to extract files on wireshark : File > Export Objects > TFTP


![Screenshot 2023-12-20 190158](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/6f0f89b3-4b78-47e5-95c0-e6a924c6d849)

saw the contents of the file named "instrutions.txt" which had a encoded message so, tried using decoding with rot13.com 


![Screenshot 2023-12-20 190305](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/e8a9c42b-7dbf-4270-a421-3d86015aea85)

![Screenshot 2023-12-20 190355](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/b86fd458-bdfe-4924-b947-d6b4f8663428)

which said " TFTP DOESNT ENCRYPT OUR TRAFFIC SO WE MUST DISGUISE OUR FLAG TRANSFER.FIGURE OUT AWAY TO HIDE THE FLAG AND I WILL CHECK BACK FOR THE PLAN"

opened another file named "plan" which also had a rot13 encoded message :


![Screenshot 2023-12-20 190641](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/0967f1b2-d3bf-43f8-86df-bd88f620c702)

![Screenshot 2023-12-20 190702](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/cbc0cede-efa8-45c9-b5ff-a215bb0a90e7)



which said "I USED THE PROGRAM AND HID IT WITH DUEDILIGENCE.CHECK OUT THE PHOTOS"

With "DUEDILIGENCE" as the password, steghide revealed there's a flag.txt hidden inside picture3. Using steghide extract -sf picture3.bmp and "DUEDILIGENCE" as the password, flag.txt was extracted.

used a command "cat flag.txt" to see the contents of the file which gave the flag :

FLAG :

picoCTF{h1dd3n_1n_pLa1n_51GHT_18375919}

