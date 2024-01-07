## credstuff


### Approach :

There were two text files given in the question. One contained the usernmes and the other contained the passwords with respect to it.

And as the question asked about the password of "cultiris" so, found out this username in the file. 
It was present on the Line 378 :

![Screenshot 2023-12-31 163446](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/75fbad75-e0c6-4ee1-89f4-d6b7279ac1d9)

so, navigated to Line 378 of the password text file and found this :

![Screenshot 2023-12-31 163500](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/86eacf9f-5e15-4be0-bdb9-b59073484e2e)

This needed to be decoded so, used rot13.com to find the flag :

![Screenshot 2023-12-31 163545](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/a320f09a-b930-4fdf-91bb-0677798bb5a0)



### FLAG :

picoCTF{C7r1F_54v35_71M3}
