# 2.Users and Groups
* The Active Directory Environment
# Objectives/ Notes
* Create OU Structure
  - The OU structure is a small scale replica of what I see everyday on the job, you can obviously get pretty technical with how you manage your OUs but I wanted to keep it as simple as possible before I get into the really important stuff. So we have "Staff" folders that dive into the employee type, a folder for "Workstations" to hold all the clients, and then one for "Servers."
* Create Security Groups
  - I made some simple security groups didn't dive too deep into permissions, just some basic stuff for realism and then add them to some test users.  
* Create Test Users
  - EmployeeID
    I want to automate the EmployeeIDs' to be automatically generated when new users are created, but until I configure that the EmployeeIDs' were manually created
  - Org. Information
    Did create some Org information job title, state, employer, etc. I'm to configure EntraID so when they connect it'll drop them into specific Entra dynamic groups based on this information.
* Delegate Permissions
  - RBAC and Password Reset
    Those with IT roles have specific permissions that those with the Finance roles don't have and it goes both ways. IT can reset passwords, change user account memberships, properties, etc. This goes hand in hand with the created security groups. 
* Delegate where new users and clients land
  - I ran a powershell script to have new clients and users automatically drop into their respective folders "Staff" or "Workstations" then they can be manually sorted from there as needed.
* Domain Security Policies
  - Account Lockout Threshold & Duration Configured
    Both have been configured in an effort to minimize security threats 
  - Password Policy Configured
    The longer and more complex a password the harder it is to crack

# Screenshots
- [Screenshots Folder](Screenshots)
- Due to the amount of media I have as this is my first lab I decided not to include it in the Docs section, once I start doing more and more labs I will slowly reduce the amount of photos and only highlight the bigger or more complex changes. It will become more coherent and flow better in the future. 
