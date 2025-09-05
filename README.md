# Hosting-Web-application-on-AWS
1. Launch an EC2 Instance

Log in to AWS Management Console → go to EC2 service.

Click Launch Instance → choose Amazon Linux 2 (or Ubuntu).

Select an instance type (e.g., t2.micro for free tier).

Launch with a key pair for SSH access.

2. Connect to the instance using SSH
   ssh -i mykey.pem ec2-user@<EC2-Public-IP>


3. Update ubuntu
   sudo apt update
   
4. Install a web server(ngnix or apache)
#Installing ngnix
sudo apt install ngnix

6.  Deploy Your Web Application
   Html File will be available on below path by default.
/var/www/html/

 7. fetch the html file present on above path
 cd /var/www/html/ ls
index.nginx-debian.html

 9. Remove the file
     rm -r index.ngnix-debian.html

 10. REcreate afile and write the code for application
sudo nano index.html

 11. File will get opened--Write the code in the file
Hello World.

 12. Save the file.
Ctrl+S

 13. Now  your application is live at:

http://<EC2-Public-IP>
