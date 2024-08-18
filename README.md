# Entra-ID Adding multiple users using Powershell

### Project Overview
---
This Project aims to demonstrate how to effectively create users from a user base of 1000 employees from a CSV file using Microsoft Entra ID using the Bulk Operation tool. A Powershell script will then verify that the users have been added.

### User Sources

The users used in this project were sourced from https://1000randomnames.com. The users were then adapted to a CSV template sourced from Entra ID Bulk operations - create users tool.

### Tools

- Powershell - used for confirming user import
- Microsoft Entra ID Adim Centre - Bulk Operations -  Create Users

### User List Preparation

![Screenshot 2024-08-17 112106](https://github.com/user-attachments/assets/c879237a-61f4-447e-a807-d9a9dd26ba92)


### Bulk Uploading Using Bulk Operations

I used the bulk operation tool to import the 1000 users into Entra ID.

https://github.com/user-attachments/assets/abf2d241-efa8-473e-b3d0-310e7f469aec



### User Analysis using Powershell

I will now verify that all 1000 users have been successfully uploaded on Entra ID using the below PowerShell script:

```powershell
Get-MgUser -Filter "UserType eq 'Member'"
```

The bekow screenshot confirms the success:

![Screenshot 2024-08-17 133209](https://github.com/user-attachments/assets/b78bec12-3715-4f87-8702-a043d2232074)


### Results

1. succesfully importsnt 1000 Users on Entra ID
2. Succesfull verified thr creation of 1000 users using Powershell

   


### References

1. https://1000randomnames.com/
2. https://learn.microsoft.com/en-us/entra/identity/users/users-bulk-add
