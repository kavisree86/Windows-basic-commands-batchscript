# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 




# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.


## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\MyLab
![image](https://github.com/kavisree86/Windows-basic-commands-batchscript/assets/145759687/0d4f5e8e-2c84-4ecd-b042-261ec2157b3a)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab
![image](https://github.com/kavisree86/Windows-basic-commands-batchscript/assets/145759687/b625a14d-9e8d-41f3-a408-cb48e2239b4b)
![image](https://github.com/kavisree86/Windows-basic-commands-batchscript/assets/145759687/8254b980-5427-4b92-a231-91a2bfd92e95)


List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab
![image](https://github.com/kavisree86/Windows-basic-commands-batchscript/assets/145759687/8a133394-7d9a-48b3-8d9f-25eddc53beb7)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
mkdir %userprofile%\Desktop\MyLab
![image](https://github.com/kavisree86/Windows-basic-commands-batchscript/assets/145759687/39588cf5-9c51-4fd4-8720-5b7626334fdf)
![image](https://github.com/kavisree86/Windows-basic-commands-batchscript/assets/145759687/61fcab53-aef8-48d2-895a-aed612c18c71)




## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab
mv Myfile.txt %userprofile%\Documents

![image](https://github.com/kavisree86/Windows-basic-commands-batchscript/assets/145759687/8f1d6b5e-f90c-4236-b63b-85214861c8b7)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

@echo off   
mkdir %userprofile%\Desktop\DocBackup   
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup   
echo Backup completed successfully!   

@echo off   
mkdir %userprofile%\Desktop\DocBackup    
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup   
del %userprofile%\Documents\*.docx    
echo Backup and deletion completed successfully!   





## OUTPUT

![image](https://github.com/kavisree86/Windows-basic-commands-batchscript/assets/145759687/7c77627e-2ffb-41be-9843-5392100456ec)




# RESULT:
The commands/batch files are executed successfully.

