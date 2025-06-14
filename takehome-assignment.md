# Take Home Assignment - Day 1 Devops Aws

# 1. Created VPC
<img width="960" alt="1" src="https://github.com/user-attachments/assets/a6bd2e92-5323-4835-ba44-a3783fb86f3e" />

# 2. Public Subnet
<img width="960" alt="2 pub-subnet" src="https://github.com/user-attachments/assets/be0ec079-9239-4cc9-ba10-1e94806276b1" />

# 3. Private Subnet
<img width="959" alt="3 priv-subnet" src="https://github.com/user-attachments/assets/bc1b0d74-ee5f-4025-bc25-36c8eb61ea61" />

# 4. Internet Gateway
<img width="960" alt="4 internet gateway" src="https://github.com/user-attachments/assets/f3db9c67-13d9-47a8-a159-c5d9d215a446" />

# 5. Connecting internet gateway to public subnet through route table
<img width="960" alt="5 internet gateway to public subnet" src="https://github.com/user-attachments/assets/a422a826-ae91-49c4-89f4-998794558c59" />

# 6. Created security group for web-server
<img width="960" alt="6 web server sg" src="https://github.com/user-attachments/assets/9b62f389-64d2-4635-83be-ae15bc3c39a5" />

# 7. Created security group for database 
<img width="960" alt="7" src="https://github.com/user-attachments/assets/5f776d79-54e5-4568-8075-dc610dff6910" />

# 8. database security group
<img width="960" alt="8" src="https://github.com/user-attachments/assets/333d49b4-7b3c-49d3-b63c-1cfd46229d9a" />

# 9. Inbound rule for database security group
giving id of the web server security group in the custom section of database group for inbound rules, so that only the web-server can access the database, which is required for this project.
<img width="955" alt="9" src="https://github.com/user-attachments/assets/e818b1a9-5f1a-4b27-9964-3db85c7629b9" />

# 10. Launching ec2 instance to run the web-server.
<img width="960" alt="10 ec2 pub" src="https://github.com/user-attachments/assets/6f970eda-5f85-447e-982a-a2e284dfe0a5" />

# 11. running web server on public ip
<img width="960" alt="11 webserver running" src="https://github.com/user-attachments/assets/c0daafbc-9895-4ab1-9725-cf461217b299" />

# 12. Launching ec2 instance for the database 
<img width="960" alt="12" src="https://github.com/user-attachments/assets/2dfa9aa8-1c9f-4a59-97c6-0bef4f33e54d" />

# 13. Both instances running
<img width="960" alt="13" src="https://github.com/user-attachments/assets/0209d54d-957f-49d4-bd5c-43857962b369" />

# 14. Instance details of database
we can see there is no public ip, as we dont want it to get accessed publicly
<img width="960" alt="14" src="https://github.com/user-attachments/assets/d4788b18-fda2-4bbb-b737-d6cc55369fd7" />

# 15. Trying to ssh into web-server ec2 instance
with a simple cli command to ssh, I am trying to ssh, I speacified the location of my .pem file which is required, and the public ip of the ec2 instance.
<img width="670" alt="15" src="https://github.com/user-attachments/assets/3fd4c6c6-bd73-4343-b28e-4742285098b5" />

# 16. Finally we are able to enter into our linux virtual machine!!!
<img width="670" alt="16" src="https://github.com/user-attachments/assets/7880074c-cbff-40f4-985d-554a3994a13d" />

# 17. Trying to ping the database
Now I am trying to ping the database which is running in private subnet, with secure inbound rule, which can only be accessed by the web server which is running in public subnet in the same vpc.
<img width="671" alt="17" src="https://github.com/user-attachments/assets/c1d09a6c-0f3c-4ec0-9f1b-63b4ce06520d" />

# 18. Not getting any packets back
This is happening because we have not set any inbound rule like icmp, only we allowed mysql/aurora, we can access the data but pinging will not happen without ICMP. That is why we are getting 100% packets loss
<img width="951" alt="18" src="https://github.com/user-attachments/assets/80281634-82a6-4684-9e65-8f7d8f8e34ea" />

# 19. cleanup process
I repeated the same steps, I did in the class assignment, step by step I deleted the instances, then detach and delete the internet gateway, then subnets, and finally vpc. same screen shots are present in the class-assignment.md file. so I didnt put them again, in this project only deleting the private subnet is extra step.

# bonus challenge

Nat gateway




