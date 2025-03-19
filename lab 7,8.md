Experiment 4


Question
Create the /home/consultant directory.
Add write permission to the consultant group. Use the 
symbolic method for setting the appropriate permissions.
Forbid others from accessing files in 
the /home/consultant directory. Use the octal method for 
setting the appropriate permissions.
Change the default umask for the operator1 user. The new 
umask prohibits all access for users that are not in their 
group. Confirm that the umask is changed.


Step1:
 Creating the /home/consultants Directory
The mkdir command is used to create the directory.

Command:
sudo mkdir /home/consultants

Step2:
Adding Write Permission to the consultants Group
The chmod command with the symbolic method is used to grant write permissions to the group.

Command:
sudo chmod g+w /home/consultants

Step3:
Restricting Access for Others
The chmod command with the octal method is used to restrict access for others.

Command:
sudo chmod 770 /home/consultants
Explanation:
770:
7 (owner): Full permissions (read, write, execute).
7 (group): Full permissions (read, write, execute).
0 (others): No permissions.

Step4:
Verifying Directory Permissions
The ls -ld command is used to check the permissions of the directory.

Command:
ls -ld /home/consultants

Step5:
Confirming the Updated umask
To confirm the new umask, create a file and a directory, then check their permissions.

Commands:
touch testfile
mkdir testdir
ls -l


Conclusion
In this lab, you practiced:

Creating directories and managing their permissions using symbolic and octal methods.
Restricting access to specific users and groups.
Configuring the umask to control default permissions for files and directories.

Snippets:

![WhatsApp Image 2025-03-19 at 20 22 17_a86ace14](https://github.com/user-attachments/assets/ac589955-4f04-487e-a1dc-8b0dbb2c3a21)

![WhatsApp Image 2025-03-19 at 20 22 18_022b4740](https://github.com/user-attachments/assets/e4db8bfd-a8c8-4996-9654-d859aa481b8d)

![WhatsApp Image 2025-03-19 at 20 22 18_f552d323](https://github.com/user-attachments/assets/f56f77cf-c476-417f-acf3-c73bb6b3e1d1)
