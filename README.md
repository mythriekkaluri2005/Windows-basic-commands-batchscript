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
```
DEVELOPED BY:EKKALURI MYTHRI             
REG.NO:212223240034   
```

# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.


## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\MyLab

![image](https://github.com/mythriekkaluri2005/Windows-basic-commands-batchscript/assets/150231422/821fb4c2-1285-4aad-b840-3ce76d98c236)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab

![image](https://github.com/mythriekkaluri2005/Windows-basic-commands-batchscript/assets/150231422/9db593c7-a51b-4c85-8ca5-8f7a9ee26610)

![image](https://github.com/mythriekkaluri2005/Windows-basic-commands-batchscript/assets/150231422/7a2d71d1-8df9-4f61-833b-3efb00cc7d81)


List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab

![image](https://github.com/mythriekkaluri2005/Windows-basic-commands-batchscript/assets/150231422/827b31d9-041b-476a-858a-9848dca91e2a)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup
copy MyFile.txt %userprofile%\Desktop\Backup

![image](https://github.com/mythriekkaluri2005/Windows-basic-commands-batchscript/assets/150231422/6d266120-c977-44ef-b6b9-a4debedd9546)

![image](https://github.com/mythriekkaluri2005/Windows-basic-commands-batchscript/assets/150231422/f199733d-c329-47ae-9a8c-ef7e0a89c7a0)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents

![image](https://github.com/mythriekkaluri2005/Windows-basic-commands-batchscript/assets/150231422/3d97d588-cc5f-4e4e-8894-b5cfb0275d80)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```
## OUTPUT

![image](https://github.com/mythriekkaluri2005/Windows-basic-commands-batchscript/assets/150231422/64608bd2-ab54-42fe-ae3a-dd5c665e5bdd)




# RESULT:
The commands/batch files are executed successfully.

