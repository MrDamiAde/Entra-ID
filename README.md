# Entra-ID Adding multiple users using Powershell

### Project Overview
---
This project demonstrates the process of efficiently creating 1,000 users in Microsoft Entra ID using a CSV file and the Bulk Operation tool. A PowerShell script is then used to verify the successful creation of these users

### User Sources

- The names used in this project were sourced from https://1000randomnames.com.
- The names were then adapted to a CSV template sourced from Entra ID Bulk operations.

### Tools

- Powershell - used for confirming user import
- Microsoft Entra ID Adim Centre - Bulk Operations -  Create Users

### 1. User List Preparation

![Screenshot 2024-08-17 112106](https://github.com/user-attachments/assets/c879237a-61f4-447e-a807-d9a9dd26ba92)


### 2. Bulk Uploading Using Bulk Operations

I used the bulk operation tool to import the 1000 users into Entra ID.

https://github.com/user-attachments/assets/abf2d241-efa8-473e-b3d0-310e7f469aec



### 3. User Analysis using Powershell

I will now verify that all 1000 users have been successfully uploaded on Entra ID using the below PowerShell script:

```PowerShell
Get-MgUser -Filter "UserType eq 'Member'"
```

The screenshot below confirms the success:

![Screenshot 2024-08-17 133209](https://github.com/user-attachments/assets/b78bec12-3715-4f87-8702-a043d2232074)


### Results

1. Successfully created 1000 Users in Entra ID
2. Verified the creation's success using Powershell

   


### References

1. https://1000randomnames.com/
2. https://learn.microsoft.com/en-us/entra/identity/users/users-bulk-add
