![1](https://user-images.githubusercontent.com/125752406/219944125-8a5b186f-d035-41b9-8be6-7741b81e7516.png)

Solution:- 
THe question gave me a RSA cipher text with really small value for e.

![2](https://user-images.githubusercontent.com/125752406/219944137-35439d41-6c08-4de4-a834-a3e107abd42b.png)

As M ** e mod n =c, M ** e = tn + c, for some t.
This implies, M = iroot(tn+c, e). So we just need to find t. 
I then wrote a code to find t and the message.

![3](https://user-images.githubusercontent.com/125752406/219944234-588b954d-746e-4453-81c8-484036759611.png)

![4](https://user-images.githubusercontent.com/125752406/219944253-ee05c483-2fff-487d-bc39-86be102d9859.png)
