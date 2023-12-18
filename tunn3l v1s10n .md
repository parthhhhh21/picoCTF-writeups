tunn3l v1s10n :


There's no file extension so we don't actually know what type of file it is.

Let's open this with a online hex editor to check the intended file type. The first two characters are BM which indicates a BMP file.

![Screenshot (514)](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/0184360b-a8bd-407b-be47-b89eb9984eef)

Let's change the file extension to .bmp and since it still doesn't open, so compared with an actual .bmp picture and changed its contents,


![Screenshot (515)](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/f17b611e-feb2-45bc-a79a-7997b9ddc095)

and got a picture in which it says "notaflag{sorry}"

It's about 2MB in size for such a tiny image. That doesn't seem right. Height for a BMP file is at offset 0016h. I changed offset 0017h from 0x01 to 0x03.


![Screenshot (516)](https://github.com/parthhhhh21/picoCTF-writeups/assets/148140667/e84f4e62-c331-41ec-9c81-f796061e2b29)

and finally, got the full picture in which the flag was visible.

FLAG :

picoCTF{qu1t3_a_v13w_2020}




