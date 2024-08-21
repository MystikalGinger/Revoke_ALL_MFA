# Revoke_ALL_MFA
Revoke all MFA methods for users in CSV list

This script will remove the authentication methods for users in the selected CSV. This script will ask for confirmation on each user. This can be modified to not ask for confirmation if you are sure that the csv you have does not include any accounts you do not want to target. To do this you need to remove lines 30,31,& 32.

To obtain a CSV please export from Azure by 

1. Going to entra.microsoft.com and logging in as an administrator
2. Selecting All users under the users tab
3. Click add filter
4. Select Account enabled and make sure toggle button is set to "yes"
5. Hit Apply
6. Click the button at the top of the panel that reads "download Users"
7. Download the CSV from the portal once this is ready
8. This is the CSV we will reference in the script


To Remove Authentication Methods for users

1.Launch Powershell on your machine as an administrator
2. Navigate to the folder where you the Revoke_MFA_365.ps1 file is stored
	For example CD "c:\users\youruser.name\downloads\Revoke MFA all users" (replace the path with wherever you have it stored)
3.run the powershell command by issuing the following command "./"revoke MFA all Users"
4. Follow the prompts
5. Sign in with global admin when prompted
6. The script will ask you for each user if you want to remove authentication methods for that user, select Y to remove and N to skip 
7. The end
