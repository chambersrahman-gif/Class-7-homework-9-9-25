
------------------------------------------------------------
Steps to Launch an EC2 Instance
------------------------------------------------------------
1. Navigate to EC2 in the AWS Console.
2. Create a new Security Group.
3. Click "Launch Instance".
4. Leave default "Amazon Linux 2023 AMI". If not already the default, then click "Amazon Linux 2023 AMI"
5. Leave the default "t2. nano". If not, choose "t2.nano" as the instance type.
6. Create and download a new key pair (used for SSH).
7. In Network Settings, choose "Select existing security group" 
   and select the custom EC2 Security Group you created.
8. Expand "Advanced Details".
   - Open startup_script.txt from GitHub.
   - Copy the plain text.
   - Paste it into the "User Data" field.
9. Launch the instance.
10. Copy the Public DNS once the instance is running.
    - Paste it into your notes.
    - Add "http://" in front to make it a usable link.


------------------------------------------------------------
Tear Down Instructions
------------------------------------------------------------
1. In the EC2 Console, click "Instances".
2. Select your instance.
3. From "Instance State", choose "Terminate Instance".
4. (Optional) Delete your custom Security Group.
