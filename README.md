# J. Dawk - Class 7: Zion Notes


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

# Homework-Week-2
Setup Instance Template
1. Create EC2 (follow previous steps)
2. Create Template From Instance
   - Select "Actions" > "Image And Templates" > "Create Template From Instance"
   - Create Launch Template. Be sure to give relevant name. eg.EC2InstanceTemp
3. Go Back to EC2 menu
   - Launch New Instance, click "down arrow menu"
   - Select Lanch Instance From Template > Select the template you named as source template. Review settings.
   - Launch Instance!

# Homework-Week-3
Command line- File Managament - GitHub
1. Upload sample files from your computer to GitHub -- Open Bash for Windonws OS, Termminal for Mac OS
2. Indentify desired location in Finder
3. Point A = Print Working Directory = "pwd" shows what folder you are currently working from.
4. Type "ls" to "get list" of what is in the current operationing folder.
5. Change directory with "cd" - *space* - [type name of target directory] - check if the path is intended
6. "clear" cleans up screen
7. "cd .." to go Up a directory (eg Class 7 > TheoWAF)
8. "cd [fileNmae]/" in Basd Windows OS to create NEW folder
9. "cd C:\" takes you to the C Drive; the basis for all of your computer files.
10. "cd users" find User name
11. "touch" to create a file (there are ways to change the file,  but "touch creates .txt file"
12. TIP: "rm [fileName]" to remove file. Do not use rm in Root ie your computers C drive. You will format your CPU if you do that!(YIKES!)
13. "mkdir [fileName]" in Terminal Mac OS to create NEW folder
14. Go into file that you created and enter: "My destination country is {country} My net income is {income] My house hous abroad has [house details] My mode of transportation is [insert vehicle]. My bed thread count is [insert bed thread count lol]. DON'T COPY ROB!!
15. insert file of a Baddie
16. "touch notes.txt" -- insert class notes
17. Go into GitHub.com > Create Repository > Copy and save link "...or create a new repository on the command line."

18. ### Initial Git Configuration

1. **Set Your Name:**
   ```bash
   git config --global user.name "JDawk-TX"
   ```

2. **Set Your Email:**
   ```bash
   git config --global user.email "230279512+JDawk-TX@users.noreply.github.com"
   ```
     Tip: Use noreply email provided by GitHub to avoid spam and safety issues.
     GitHub > "Settings" > "Email" > Toggle ON "Keep my email address private"

4. **Verify Configuration:**
   ```bash
   git config --global --list
   
5. ### Basic Git Workflow
To check file status localy = "ls"
To check file stutus on GitHub = "git status"
  It will show which files are queued to be PUSHED/"commited" to GitHub (Green = Ready, Red = NOT Ready)

```bash
git init
git add <files to stage>
git commit -m "<First Commit>"
git branch -M main
git remote add origin https://github.com/JDawk-TX/9.23.25_class7_JDawk
git push -u origin main

Create SSH keys for LOGIN
ssh-keygen -t ed25519 -C "jddawkins3@protonmail.com"
