## Magikarp Ground Mission

### Approach :

Connected to the shell via online ssh with :


user :- ctf-player

host :-venus.picoctf.net

port :- 58277

password :- abcba9f7


![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/ef4f02f1-d4af-445d-a153-aefd54788e86)

used a command 'ls' which shows the contents of the current directory and got two files :


![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/8075d6ef-7a60-499a-abb1-ef9983c912eb)

extracted the first part of the flag by using the command "cat 1of3.flag.txt" which shows the contents of the files :

![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/2e3cf71b-cf60-4855-87ae-49229bb55c6c)

again used the cat command :


![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/e7d07dcf-9edc-41b8-af46-ed40ab57fff7)

but here, it said to go to the root directory as the instructions in order to find the next part of the flag, so used the cd command which changes the current working of the directory :



![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/ba8e220f-6593-4b60-9b4d-667f57cedeb8)

In the root directory, saw a "2of3.flag.txt" file which I cat out to get the second part of the flag :

![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/ff610609-0a34-4840-b5be-bf77fb23c17d)

 Used the instructions given and change to the home directory which is also often represented by this symbol "~" :


 ![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/33f8d1cd-8a40-4aad-9942-17fab9dc1d69)

 Used the ls command and saw the final part of the flag file. So, used the cat command to get that final part :


 ![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/08d8de25-f7da-4eeb-9eeb-a06c2aa39873)


### FLAG :

picoCTF{xxsh_0ut_0f_\/\/4t3r_21cac893}

 













