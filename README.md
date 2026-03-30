# Active Directory Bulk User Creation Lab

## Lab Overview
This lab demonstrates how to perform **bulk user creation** in Microsoft Active Directory using PowerShell.  
Bulk user creation saves time and ensures consistency when adding many users to an AD environment.


**Environment:** Windows Server with Active Directory module / Azure AD

---

## Lab Scenario
Your organization is onboarding a large group of employees. Instead of creating users individually:  
- Users will be created from a CSV file.  
- Users will be assigned to specific organizational units (OUs) and groups.  
- This lab simulates a production-like environment for testing bulk operations.

---

## Lab Architecture
![Bulk Upload Architecture](images/bulk-upload-example.png)

---

## Lab Tasks

### Task 1: Prepare User Data
1. Create a CSV file (`sample-users.csv`) with the following headers:

```csv
FirstName,LastName,UserName,Password,OU
John,Doe,jdoe,P@ssword123,OU=IT,DC=corp,DC=local
Jane,Smith,jsmith,P@ssword123,OU=HR,DC=corp,DC=local
