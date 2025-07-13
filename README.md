# Building App-Server-using-Node.js in RHEL 9.5

## 1. Update the System
```
sudo dnf update -y

#dnf: The default package manager in RHEL 9+ versions

#update: Updates all installed packages to the latest available version.

#-y: Automatically answers "yes" to all prompts.
```
![alt text](image.png)

## 2. Enable and Install Node.js
```
sudo dnf module list nodejs

#Lists all available streams (versions) of Node.js
```
![alt text](image-1.png)

```
sudo dnf module enable nodejs:18 -y

#module enable: Activates a specific version stream of Node.js (version 18 here).

#-y: Confirms the enablement.
```
![alt text](image-2.png)

```
sudo dnf install nodejs -y

#Installs Node.js and its package manager
```
![alt text](image-3.png)
![alt text](image-4.png)

```
node -v
npm - v 

#Verifies installation by printing the installed versions of Node.js and npm.
```
![alt text](image-6.png)

## 3. Create a Project Directory 

```
mkdir ~/my-node-app-server
cd ~/my-node-app-server

#mkdir: Creates a new directory called my-node-app in your home directory.

#cd: Changes into that directory.
