Exercise 2: Work with CloudShell
----------------------------------

**2.1 Launch Cloud Shell**

1. Select the **Cloud Shell** from the upper right corner of the Azure Portal. 

   <img src="images/azureclisign.png"/><br/>

2. Select **BASH** in cloud shell window.<br/>

3. Select **Show Advance Setting**.<br/>

4. Create a storage accounr for Bash, provide unique name for **Storage Account**, **File share** and then click on **Create Storage**.<br/>

   <img src="images/bashst.png"/><br/>
 
 **2.2 Get Public IP of VM using az cli**
 
 Run following command to get **Public IP** of your virtual machine.
   - g :- Enter you **Resource Group** name.<br/>
   - n :- Enter  your **Virtual Machine** name.<br/>

  
  ```
  az vm show -d -g ODL-linux-XXXX -n VMname --query publicIps -o tsv
  ```
      
**2.3 SSH to VM using Public IP**

1. Run below command to take **SSH** of your virtual machine.
   - x.x.x.x :- Replace this with your virtual machine **Public IP**.

  ```
    ssh azureuser@x.x.x.x
   
  ```
   <img src="images/ssh.png"/><br/>
   
 **2.4 Perform basic operation inside VM**

   <img src="images/task.png"/><br/>
   
  
---------------------------------------------------------------
 
