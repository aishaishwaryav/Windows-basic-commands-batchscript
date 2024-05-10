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
![image](https://github.com/aishaishwaryav/Windows-basic-commands-batchscript/assets/151565589/0d1c931c-0132-467e-a239-1a645505b196)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/aishaishwaryav/Windows-basic-commands-batchscript/assets/151565589/f2ae583f-91e3-49ac-bdcf-959749805451)

```
type nul > MyFile.txt
```
![image](https://github.com/aishaishwaryav/Windows-basic-commands-batchscript/assets/151565589/6a8337f0-c88f-4b81-a611-16e5f0bec7f7)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/aishaishwaryav/Windows-basic-commands-batchscript/assets/151565589/066144e3-43b8-4d7c-bf48-8a03d75d6c7e)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup
```
![image](https://github.com/aishaishwaryav/Windows-basic-commands-batchscript/assets/151565589/7a228e90-8940-43be-8231-4766db062bb7)

```
copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/aishaishwaryav/Windows-basic-commands-batchscript/assets/151565589/e045c571-5703-455a-8d32-9aa6b2a2afde)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Documents

move MyLab Documents
```
![image](https://github.com/aishaishwaryav/Windows-basic-commands-batchscript/assets/151565589/6b0dcb2a-0b98-4712-ac5a-4d558ca37037)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

# COMMAND:
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
![image](https://github.com/aishaishwaryav/Windows-basic-commands-batchscript/assets/151565589/0594a6df-84d8-4328-a347-5e6ca215a41c)

# COMMAND:
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```

## OUTPUT

![image](https://github.com/aishaishwaryav/Windows-basic-commands-batchscript/assets/151565589/27953f04-f5d1-4b1f-a369-60b6cb1d90e1)


# RESULT:
The commands/batch files are executed successfully.

