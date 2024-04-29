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

Developed by:Vineela Shaik<br>
RegisterNumber:212223040243


# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.
```
mkdir %userprofile%\Desktop\MyLab
```

![image](https://github.com/ahalyaselvakumar/Windows-basic-commands-batchscript/assets/144870759/a8ba7474-2735-44e2-9c65-d7c790b07874)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/ahalyaselvakumar/Windows-basic-commands-batchscript/assets/144870759/f6cfcef6-e0ed-4d72-8a7b-c8f66e2e3116)

![image](https://github.com/ahalyaselvakumar/Windows-basic-commands-batchscript/assets/144870759/15ddb7d8-bd0b-4a9a-a7aa-053fc3aaac53)


## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```

![image](https://github.com/ahalyaselvakumar/Windows-basic-commands-batchscript/assets/144870759/82fcf333-fd7b-41b0-84ec-0c7bd1019de9)


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/ahalyaselvakumar/Windows-basic-commands-batchscript/assets/144870759/c1492ba3-8846-47e4-8764-a9a76381017b)

![image](https://github.com/ahalyaselvakumar/Windows-basic-commands-batchscript/assets/144870759/f6fa92fe-c256-4156-916d-60ba3b711df9)

## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```

![image](https://github.com/ahalyaselvakumar/Windows-basic-commands-batchscript/assets/144870759/d22389c5-7ddd-4d84-b5da-bbd85a18bd94)


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

![image](https://github.com/ahalyaselvakumar/Windows-basic-commands-batchscript/assets/144870759/622fa742-3a27-4a68-8424-03e8d79660f5)


# RESULT:
The commands/batch files are executed successfully.

