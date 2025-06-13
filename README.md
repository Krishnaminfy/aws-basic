# aws-basic

In this assginment I have launched an EC2 instance. 

# 1. created the key pair 

<img width="960" alt="1 key pair" src="https://github.com/user-attachments/assets/3b161c03-4bb1-4102-b4e2-df2366dadaa2" />
<img width="960" alt="2 key pair" src="https://github.com/user-attachments/assets/5fdd78ce-234f-4ad8-83c8-093625c2373a" />

# 2. created a vpc to run EC2 instance inside it.
<img width="960" alt="3 vpc" src="https://github.com/user-attachments/assets/fc133f5f-13b6-49a9-88cf-f38f1657eebf" />

# 3. created the public subnet to communicate with internet.

<img width="960" alt="4 subnet" src="https://github.com/user-attachments/assets/5ac42095-959d-42ee-9674-b1607c26bc00" />

I have created internet gateway to work as a door for allowing in and out of public internet
<img width="960" alt="6 internet" src="https://github.com/user-attachments/assets/c7f65a32-4f74-474c-b226-b5a602c1e1ec" />

# 4. After creating vpc, I got this route table which was already connected to the vpc, so I just edit the routes to connect it to the internet gateway and, also associate my public subnet
<img width="960" alt="7 routetable" src="https://github.com/user-attachments/assets/244313dc-2446-4bc2-86f3-d5faf0f1c74a" />
<img width="960" alt="8 route table" src="https://github.com/user-attachments/assets/83ca0737-544d-46d8-bdc9-2af1981344e8" />

# Then I created the security group for the ec2 (firewall), in which I have allowed http for any ipv4 and ssh for my ip only
<img width="960" alt="9 sg" src="https://github.com/user-attachments/assets/6955a4e0-d8d7-4f1a-88fb-2a114a05b5c2" />


<img width="960" alt="10" src="https://github.com/user-attachments/assets/d81ead5a-d549-436a-bc6e-1f1e0dace8c8" />

# Now my ec2 instance is running!!
<img width="960" alt="11" src="https://github.com/user-attachments/assets/15ee0a07-afba-489b-bae5-44f8af8e8793" />

<img width="960" alt="12" src="https://github.com/user-attachments/assets/dedf4814-5d4e-4c2b-9065-fc5591b58301" />

<img width="960" alt="13" src="https://github.com/user-attachments/assets/eac69f8b-d4b6-402b-9ed4-fac6ac52114b" />

# Cleanup processes
<img width="960" alt="14" src="https://github.com/user-attachments/assets/02554dcb-35a9-4bc6-b420-8e8ed5170adc" />
<img width="960" alt="15" src="https://github.com/user-attachments/assets/67d85e32-bb74-4e4f-889f-922bc587a969" />

<img width="960" alt="16" src="https://github.com/user-attachments/assets/662aa38c-142f-44ad-bbe4-ded7fa7e0c77" />

<img width="960" alt="17" src="https://github.com/user-attachments/assets/98d53176-adaa-41d8-a0d4-ac3837a6426a" />

<img width="960" alt="18" src="https://github.com/user-attachments/assets/a614ba1c-72eb-4dc6-b9f0-2652b1637fdb" />

<img width="960" alt="19" src="https://github.com/user-attachments/assets/4adb714c-7318-478b-b92d-6673a8ca67ea" />

<img width="960" alt="20" src="https://github.com/user-attachments/assets/98227278-54b5-42f0-954a-90044aa3f7d6" />




<img width="960" alt="21" src="https://github.com/user-attachments/assets/8e592b69-0338-47d9-a23c-955735d2ead7" />



<img width="960" alt="22" src="https://github.com/user-attachments/assets/9c3105a6-457b-4a90-8c00-f39d19d6cd1a" />








