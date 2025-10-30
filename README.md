### Windows-basic-commands-batchscript
## Ex08-Windows-basic-commands-batchscript

### AIM:
To execute Windows basic commands and batch scripting

## DESIGN STEPS:
### Step 1:
Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware

## Step 2:
Write the Windows commands / batch file Save each script in a file with a .bat extension. Ensure you have the necessary permissions to perform the operations. Adapt paths as needed based on your system configuration.

## Step 3:
Execute the necessary commands/batch file for the desired output.

## WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.
```
mkdir %userprofile%\Desktop\MyLab
```
<img width="690" height="52" alt="image" src="https://github.com/user-attachments/assets/c3497d88-769c-44df-b1b8-5db890077f44" />

## COMMAND AND OUTPUT
Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

## COMMAND AND OUTPUT
List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
<img width="777" height="127" alt="image" src="https://github.com/user-attachments/assets/1221f006-5b6f-466a-894e-d22580a6dc66" />


## COMMAND AND OUTPUT
Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```


## COMMAND AND OUTPUT
Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
<img width="793" height="135" alt="image" src="https://github.com/user-attachments/assets/7e740338-e0d1-44a2-9d67-f8181648cba4" />


## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
<img width="747" height="47" alt="image" src="https://github.com/user-attachments/assets/7a146957-1e71-4490-8d84-1ac0addae970" />


# Exercise 2: Advanced Batch Scripting
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
<img width="642" height="86" alt="image" src="https://github.com/user-attachments/assets/d5dc8e2c-d460-44f4-85b5-9572d9800b08" />


## RESULT:
The commands/batch files are executed successfully.
