## Exercise 2:- Work with CloudShell

1. Select the **Cloud Shell** from the upper right corner of the Azure Portal. 

   <img src="images/azureclisign.png"/><br/>

2. Select **BASH** in cloud shell window.<br/>

3. Select **Show Advance Setting**.<br/>

4. Create a storage for Bash give uniqe **Storage Name** and **File share** name then click on **Create Storage**.<br/>

   <img src="images/bashst.png"/><br/>
 
 **Get Public IP of VM using az cli command**
 
 Run this command for see **Public IP** of your virtual machine.<br/>
  - -g :- Enter you **Resource Group** name.<br/>
  - -n :- Enter  your **Virtual Machine** name.<br/>

  
  ```
  az vm show -d -g ODL-Linux-XXXX -n VMname --query publicIps -o tsv
  ```
      
**SSH to VM using Public IP**

Run below command to take **SSH** of your virtual machine.
   X.X.X.X :- Enter your **Public IP**

  ```
    ssh azureuser@x.x.x.x
   
  ```
   <img src="images/ssh.png"/><br/>
   
**Perform basic operation inside VM**

  <img src="images/task.png"/><br/>
  
  
---------------------------------------------------------------
 
