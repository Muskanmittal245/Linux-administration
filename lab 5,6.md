Experiment3

Question

Use Vim,nano, to edit the editing_final_lab.txt file. Use the 
lab_file shell variable. Enter the visual mode of Vim. Remove 
the last seven characters from the first column on the first 
line. Preserve only the first four characters of the first 
column.


Step1:
 Preparing the Lab File
Ensure the file editing_final_lab.txt exists. If not, create it using:
touch editing_final_lab.txt
To simplify file access, store its path in a shell variable:
lab_file="editing_final_lab.txt"

Step2:
Editing with Nano
Nano is a beginner-friendly text editor.

Steps:
Open the file in Nano:
nano $lab_file
Add the following lines:
Hello world!

Snippets:
![WhatsApp Image 2025-03-19 at 20 08 09_b6fdfd94](https://github.com/user-attachments/assets/caeb247b-90f9-46e0-9b28-e9ce89764431)

Step3:
Editing with Vim
Vim is a powerful text editor with advanced features.

Steps:
Open the file in Vim:
vim $lab_file
Delete the Last Seven Characters of the First Line:
Enter visual mode (v), highlight the last seven characters, and press d.
Keep Only the First Four Characters of the First Line:
Move to the start of the line, press 4l, enter visual mode (v), highlight the rest, and press d.
Save and exit:
Press ESC, type :wq, and press Enter.

Snippets:
![WhatsApp Image 2025-03-19 at 20 08 09_b420d652](https://github.com/user-attachments/assets/2cde53c5-2a4a-4d68-96a9-bb64584157b0)


Step4:
Verifying Command Execution
To confirm the changes, display the file's contents:

cat $lab_file
Screenshot:
Verifying File Contents

Expected Output:
If the file initially contained:
hello world!

After editing with Vim, the first line should appear as:

Snippets:
![WhatsApp Image 2025-03-19 at 20 08 09_820caf24](https://github.com/user-attachments/assets/220a05b3-81d1-48ac-b272-dd18ef0ca109)


Conclusion:
In this lab, you learned how to:

Use Nano for basic file editing.
Use Vim for advanced text manipulation, including deleting specific characters and retaining selected portions 
