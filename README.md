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
```
mkdir %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/a5f6cb22-c46c-43d4-b7c0-bfd432937b1c)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/e0f1c0bb-6f31-48e3-ac5e-eb9d5579b107)
```
type nul > MyFile.txt
```
![image](https://github.com/user-attachments/assets/fbd078eb-7499-403a-abde-cc87750c25c1)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/dbfe99cc-a1e9-4a8d-8e2e-dcb1d2cd710d)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup
```
![image](https://github.com/user-attachments/assets/1e6ac046-8b39-47d1-a503-416f7fb7c4d9)
```
copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/user-attachments/assets/2968bc38-9331-4e23-8abc-f3d83f39d4db)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Documents
move MyLab Documents
```
![image](https://github.com/user-attachments/assets/56bf0440-dc79-44dd-98cd-62e5a4f0fc69)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

##COMMAND
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
![image](https://github.com/user-attachments/assets/e3a4e0c8-f609-4b01-b85c-3d6267f21311)






## OUTPUT

![image](https://github.com/user-attachments/assets/a98fa09c-5d04-4eee-ad45-0af0c2f01d40)




# RESULT:
The commands/batch files are executed successfully.

