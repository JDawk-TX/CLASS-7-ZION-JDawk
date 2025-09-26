# JimmyD-Week-1-HW
# Homework-Week-1

Setup EC2
1. Create Security Group FIRST
2. Create an EC2
  -Creating key pairs. A key pair allows you to connect to that server through SSH(Secure Shell). It connects a AWS EC2 user via   SSH
  -Create the Instance without a key pair, it is less safe but it works for what we did in class.
  -Next you need to open Advanced options, and upload this bash script from the group    https://github.com/Meifumado13/bmc4/blob/main/ec2scrpit. 
    -Run the instance and this will start it up.
3. Copy public DNS, make it into a useable link, and use the link
  -Example -- http://ec2-18-224-96-168.us-east-2.compute.amazonaws.com
4. How to Close and or Terminate an Instance
  -Open instances and click the box on the left of the instance that is running and go to Instance state button on the upper  right side and click the drop down menu. Then click on either stop instance to stop it and leave it in your cloud drive or VPC. To terminate it, click the Terminate (delete) instance and this will get rid of your instance

Setup Instance Template
1. Create EC2 (follow previous steps)
2. Create Template From Instance
   - Select "Actions" > "Image And Templates" > "Create Template From Instance"
   - Create Launch Template. Be sure to give relevant name. eg.EC2InstanceTemp
3. Go Back to EC2 menu
   - Launch New Instance, click "down arrow menu"
   - Select Lanch Instance From Template > Select the template you named as source template. Review settings.
   - Launch Instance!
