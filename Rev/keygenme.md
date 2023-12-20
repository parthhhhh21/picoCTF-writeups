## Keygenme-py

### Approach :
•	This program contains the first part called key_part_static1_trial that has the first part of the flag: picoCTF{1n_7h3_|<3y_of_. The portion of the flag we need to find if key_part_dynamic1_trial.



•	The check_key functions contains the code that fills in the key_part_dynamic1_trial.


•	It takes the hexdigest of the sha256 hash of b"GOUGH" and then selects a certain character by an indexing to a certain point on that string.


•	We can simply find the hexdigest of the sha256 hash of b"GOUGH" and then get the characters at the positions it checks: "".join([hashlib.sha256(b"GOUGH").hexdigest()[x] for x in [4,5,3,6,2,7,1,8]]). This is the missing section of the flag.



![image](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/46e5d540-e29f-4295-9674-35367213f8d7)



### FLAG :


picoCTF{1n_7h3_|<3y_of_f911a486}
