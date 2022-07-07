# **Overview** 

Azure Virtual Desktop is a desktop and app virtualization service that runs on the cloud. 

Here's what you can do when you run Azure Virtual Desktop on Azure: 

 * Set up a multi-session Windows 10 deployment that delivers a full Windows 10 with scalability. 
 * Virtualize Microsoft 365 Apps for enterprise and optimize it to run in multi-user virtual scenarios. 
 * Provide Windows 7 virtual desktops with free Extended Security Updates. 
 * Bring your existing Remote Desktop Services (RDS) and Windows Server desktops and apps to any computer. 
 * Virtualize both desktops and apps. 
 * Manage Windows 10, Windows Server, and Windows 7 desktops and apps with a unified management experience. 

## **General Hierarchy** 

### **Host Pools** 

Host pools are a collection of one or more identical virtual machines within Azure Virtual Desktop tenant environments. Each host pool can be associated with multiple RemoteApp groups, one desktop app group, and multiple session hosts. Host Pools can be one of two types: 

* **Personal**, where each session host is assigned to individual users. 

* **Pooled**, where session hosts can accept connections from any user authorized to an application group within the host pool. You can set additional properties on the host pool to change its load-balancing behavior, how many sessions each session host can take, and what the user can do to session hosts in the host pool while signed in to their Azure Virtual Desktop sessions. You control the resources published to users through application groups. 

 

 

### **Application Groups** 

An Application Group is a logical grouping of applications installed on session hosts in the host pool. An application group can be one of two types: 

* **RemoteApp**, where users access the RemoteApps you individually select and publish to the application group. 

* **Desktop**, where users access the full desktop By default, a desktop application group (named “Desktop Application Group”) is automatically created whenever you create a host pool. You can remove this application group at any time. However, you can’t create another desktop application group in the host pool while a desktop application group already exists. To publish RemoteApps, you must create a RemoteApp application group. You can create multiple RemoteApp application groups to accommodate different worker scenarios. Different RemoteApp application groups can also contain overlapping RemoteApps. 

### **Workspaces** 

A workspace is a logical grouping of application groups in Azure Virtual Desktop. Each Azure Virtual Desktop application group must be associated with a workspace for users to see the remote apps and desktops published to them. 

### **End users** 

After you’ve assigned users to their application groups, they can connect to an Azure Virtual Desktop deployment with any of the Azure Virtual Desktop clients. 

# **Lab Guide Outline** 

### **Pre-requisites to deploy Azure Virtual Desktop** 

**Exercise 1: Create Host Pool from Azure Portal**

Getting Started with the Lab 

* Task 1: Log in to Azure Portal 

* Task 2: Create Host Pool 

**Exercise 2: Create Application Groups and assign to users** 

* Task 1: Create Application Group 

**Exercise 3: Access the Published Applications and Desktop using Browser**

* Task 1: Access the Published Application 

* Task 2: Access the published Desktop 

**Exercise 4: Access the Published Applications and Desktop using AVD Desktop Client** 

* Task 1: Access the Published Applications 

* Task 2: Access the Virtual Desktop 

**Exercise 5: Load Balancing methods**

* Task 1: Add new users to Azure Active Directory 

* Task 2: Update Passwords for the new users 

* Task 3: Change and experience Load Balancing methods 

## **Code Example**

```
console.log("Hello Brian!")
```
