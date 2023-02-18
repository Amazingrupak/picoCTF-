![1](https://user-images.githubusercontent.com/125752406/219901858-75642f8e-5809-4bec-9973-33e545ec223a.png)

Solution:-
It is a pptm file so I tried opening it with powerpoint. Most of the slides were empty except one saying no flag and one saying forensics is fun.

![2](https://user-images.githubusercontent.com/125752406/219901868-d4f2a8bc-2f9d-4810-b43c-5ba885640dab.png)

Then I tried wget and binwalk to see if there are any hidden files.
I foudn tons of zipped files hidden.
I used -e to extract the files.

![3](https://user-images.githubusercontent.com/125752406/219901893-7954fdb3-1fd6-47f3-8bee-3334d702a44d.png)

![5](https://user-images.githubusercontent.com/125752406/219901909-0e8d9924-f09a-4518-8633-c93cc1153e00.png)

I used grep to try and find usual words used to store flag like pico, flag, secret etc.
I finally found something useful using find -D tree|grep hidden. It gave me the output ./ppt/slideMasters/hidden.
Using cat command I found a series of letters and numbers. I used a base 64 decoder to find the flag.

![6](https://user-images.githubusercontent.com/125752406/219901921-926dbb8a-1606-42ea-97b6-f61f57873911.png)

![7](https://user-images.githubusercontent.com/125752406/219901938-39ea828a-d9f0-4686-9304-b5c02cb888f7.png)
