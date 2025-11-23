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
![image](https://github.com/user-attachments/assets/88978e9c-7baa-4ded-ba88-998d8dab019c)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
      cd %userprofile%\Desktop\MyLab
![image](https://github.com/user-attachments/assets/715142d5-e87f-42e1-9557-d0f2c6c7acf2)
      type nul > MyFile.txt
![image](https://github.com/user-attachments/assets/ab81e2eb-4d27-4153-8706-b52780bbdfd3)

List the contents of the "MyLab" directory.

## COMMAND AND OUTPUT
       dir %userprofile%\Desktop\MyLab
![image](https://github.com/user-attachments/assets/205529c4-aee8-44e5-a963-0dce19ff3647)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
      mkdir %userprofile%\Desktop\Backup
![image](https://github.com/user-attachments/assets/793b52b7-d2a0-4263-861a-a2ce3e9dd65e)
      copy MyFile.txt %userprofile%\Desktop\Backup
![image](https://github.com/user-attachments/assets/5d1b4525-31a3-4ee7-af6a-bb2aaa825f65)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
      mkdir %userprofile%\Desktop\Documents
      move MyLab Documents
![image](https://github.com/user-attachments/assets/9720bdb5-ea91-42f0-bc03-7ae8b455ed55)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

## COMMAND:

      @echo off
      mkdir %userprofile%\Desktop\DocBackup
      copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
      echo Backup completed successfully!
      
![image](https://github.com/user-attachments/assets/964b0c24-cd6f-475c-b573-8b82b5a104fe)

## COMMAND:
      @echo off
      mkdir %userprofile%\Desktop\DocBackup
      copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
      del %userprofile%\Documents\*.docx
      echo Backup and deletion completed successfully!
      


## OUTPUT
![image](https://github.com/user-attachments/assets/92514ea1-a11d-4403-b222-5939e30fc577)




# RESULT:
The commands/batch files are executed successfully.

