![1](https://user-images.githubusercontent.com/125752406/219903401-fe5e9f28-5971-4fe7-bd24-f797ac0dfdfe.png)

Solution:-
The file is a pcapng. I ran it in wireshark and extracted the files by using export objects in file menu and then saved them using save all.

![2](https://user-images.githubusercontent.com/125752406/219903407-61907a6e-dc00-43e3-a61b-223e2bde1ecc.png)

![3](https://user-images.githubusercontent.com/125752406/219903426-e5724b20-54be-4a47-868c-57c69ff3950d.png)

I also anazlysed the text and followed the udp stream. In stream 1 and 8 I found texts, encoded using ROT13.

![4](https://user-images.githubusercontent.com/125752406/219903455-765148b0-6a31-4a14-bc8c-b47598ce09ee.png)

Decoding it using ROT13.com I found two texts saying "TFTP DOESNT ENCRYPT OUR TRAFFIC SO WE MUST DISGUISE OUR FLAG TRANSFER. FIGURE OUT A WAY TO HIDE THE FLAG AND I WILL CHECK BACK FOR THE PLAN" and "I USED THE PROGRAM AND HID IT WITH - DUEDILIGENCE. CHECK OUT THE PHOTOS "

![5](https://user-images.githubusercontent.com/125752406/219903467-1aef8ddf-0698-466d-ac81-883a1902943c.png)

![6](https://user-images.githubusercontent.com/125752406/219903474-db0a6702-0000-4393-a860-4bbf0dbe58e1.png)

![1](https://user-images.githubusercontent.com/125752406/219903590-7807ab35-7614-4dc7-8e80-bc9995c7dbf5.png)

![2](https://user-images.githubusercontent.com/125752406/219903597-2eb8c85a-bd54-427f-b5c3-6cc9a0672b6b.png)

Then I went to the extracted files, copied and pasted them in my linux directories.
I then used the steghide(steghide info picture3.bmp as it was in the 3rd picture) command on the pictures. It asked me for a password. 
The text I found earlier suggested using DUEDILIGENCE as the password. I found an embedded file called flag.txt after submitting the password.

![7](https://user-images.githubusercontent.com/125752406/219903490-79e7bc17-a616-4c9d-9081-b32acfdffd85.png)

Using steghide extract -sf picture3.bmp and then giving the password as DUEDILIGENCE again, it extracetd data and wrote it in the flag.txt file. 

![8](https://user-images.githubusercontent.com/125752406/219903502-d5110a51-e854-4a2a-af95-3884e59b9d7b.png)

Openign the file in notepad gave me the flag.

![9](https://user-images.githubusercontent.com/125752406/219903515-369eea74-d79b-4338-b674-766b69a39a5e.png)
