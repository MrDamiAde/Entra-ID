# Entra-ID Adding multiple users using Powershell

### Project Overview
---
This Project aims to demonstrate how to effectively add a user base of 1000 employees from a CSV file onto Microsoft Entra ID using the bulk operation tool. A Powershell script will then be used to veridy that the users have been added.

### User Sources

The users used in this project were sourced from _____. a user template was then sourfed from Entra ID to input the user values.

### Tools

- Powershell - used for confirming user import
- Microsoft Entra ID

### User List Preparation

![Screenshot 2024-08-17 112106](https://github.com/user-attachments/assets/c879237a-61f4-447e-a807-d9a9dd26ba92)


### Bulk Uploading Using Bulk Operations

I used the bulk operation tool to import the 1000 users in 1 go.




### User Analysis using Powershell

I will now verify that all 1000 users have been successfully uploaded on Entra ID using the below PowerShell script:

```powershell
Get-MgUser -Filter "UserType eq 'Member'"
```

The bekow screenshot confirms the success:

![Screenshot 2024-08-17 133209](https://github.com/user-attachments/assets/b78bec12-3715-4f87-8702-a043d2232074)


### Results

1. succesfully created 1000 Users on Entra ID
   


### References

1. https://1000randomnames.com/
