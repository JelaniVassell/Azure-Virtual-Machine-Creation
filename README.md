![Azure preview](https://github.com/user-attachments/assets/80076bf9-d881-4aa4-b384-816db4e90447)

# ⚙Azure-Virtual-Machine-Creation
## This walkthrough will serve as a guide through the process of creating Windows and Linux virtual machines in the Microsoft Azure cloud. The entire process, step-by-step, demonstrates how to set up and configure virtual machines for hands-on experience with cloud infrastructure. 


# ⚙Environments Used
## Microsoft Azure
# ⚙Operating System 
## Windows 10 Version (22H2)
# 💻<ins> Step 1 - Create A Microsoft Azure Subscribion </ins>

## Go to https://portal.azure.com, sign in with your Microsoft account. 

## The azure free trial is based on the time window of 30 days from the account creation or whenever the $200 allotted credit runs out. If you don’t use all your credit at the end of the first 30 days, it’s lost. Alternatively, there is a pay-as-you go feature if the free trial period has ended.

# 💻<ins> Step 2 - Get logged into the Azure Portal </ins>

<img width="1859" height="873" alt="sign in azure" src="https://github.com/user-attachments/assets/c13c0a65-0627-43e8-8cf9-babe6e1c3b39" />

# 💻<ins> Step 3 - Observe the portal </ins>
## Azure services include resource groups, virtual machines, Entra ID, and more!
<img width="1659" height="894" alt="1 azure services" src="https://github.com/user-attachments/assets/9708fd9d-65ac-4de5-81f1-bf469be3e2a5" />


# 💻<ins> Step 4 - Create a Resource Group Within the Azure Portal </ins>
![1 create resourse 2](https://github.com/user-attachments/assets/b7ce37b4-0795-49b6-af7a-2a888c415903)

## Alternatively, the search bar may be used to find necessary services.
<img width="1640" height="817" alt="1 2resourse group drop down" src="https://github.com/user-attachments/assets/1e269dcf-3fa6-4ea9-92ca-b71b6d52762e" />


## Click "Create" to begin the resource group creation process.
<img width="1664" height="898" alt="3 create resourse" src="https://github.com/user-attachments/assets/ea2c676c-6704-490a-aadf-581f0ff547b3" />

## You,ll arrive upon this ⬇️ screen next. 
<img width="1663" height="925" alt="3 1 create" src="https://github.com/user-attachments/assets/18bd1e87-9b80-4bd3-9431-dc717e2524f0" />

## If you have more than one subscription, you can select the relevant one. This choice is useful to more easily separate cost if you are using Azure services for two or more businesses. 

## "Azure Subscrption 1" is my subscription of choice and my resource group is named "Lab Jelani". 
 
## The "region" selection is to choose which one of the Microsoft data centers around the would be tasked with storing your data.

## After clicking, "Next", you'll be directed here ⬇️ to chose your tags.

 <img width="1645" height="919" alt="3 2 tags" src="https://github.com/user-attachments/assets/2bf133d0-3d79-44e9-8b76-6438c3f8e469" />

## Tags are not a mandatory requirement, however, organizations may use tags to organize resources by category.
 
## Then, click "Review + Create" here ⬇️ to finish the creation.

<img width="1639" height="918" alt="3 3 review and create new" src="https://github.com/user-attachments/assets/f7e7c14c-17cf-47ae-a5a7-25dd9e2c254c" />


## You'll find your new resource group using the search function mentioned in Step 4.
<img width="1647" height="910" alt="3 4 RG created here" src="https://github.com/user-attachments/assets/85d55927-c8cb-4923-a1f9-f516d4a8e432" />

# 💻<ins> Step 5 - Create A Storage Account Within The Resource Group Created In Step 4 </ins>
## Using the search function, find "Storage Accounts" here ⬇️.
<img width="1657" height="910" alt="5  storage account search copy" src="https://github.com/user-attachments/assets/49d4e8ac-c2e7-4774-8a1b-fa2241f42b0e" />

## You'll notice that there are no storage accounts to display. Next, click "Create"
<img width="1647" height="898" alt="5 1 create one copy" src="https://github.com/user-attachments/assets/ca18c1ed-c903-4e77-94d9-7ddded767118" />

## Using your relevant subscriotion and the resource group created in Step 4, input your storage account details.
<img width="1652" height="921" alt="5 2 storage account project details" src="https://github.com/user-attachments/assets/11da04b5-53ae-4c6a-89d7-7a35088b1bab" />

## Based on the sensitivity of your data and cost efficency, choose your redundancy from this ⬇️ menu. I chose "Locally redundant storage".

<img width="1652" height="912" alt="5 3 redundance explain" src="https://github.com/user-attachments/assets/edbebdc0-8dad-470a-a7f2-ac868404447e" />


##  Next, click "Review + Create" here ⬇️.
<img width="1652" height="918" alt="5 4 review create copy" src="https://github.com/user-attachments/assets/6aa0e2ae-aace-44be-afd8-6882d31bff89" />

## You'll be directed to this ⬇️ screen to review your selections. After you have, click "Create" to continue.
<img width="1645" height="921" alt="5 5 validated and click create again page" src="https://github.com/user-attachments/assets/b466b11c-b483-4f52-b970-d3f1c6e256d4" />



## It'll take about 15 seconds for the storage account to be deployed. Wait for it to complete before moving along.
<img width="1549" height="900" alt="5 6 Validated and click page" src="https://github.com/user-attachments/assets/8f514382-a9dd-4b0d-8914-576e39b83e4d" />

## The deployment is now complete and you can view the newly created storage account within the resouce group here ⬇️.
<img width="1667" height="772" alt="5 8 CONTINUED new" src="https://github.com/user-attachments/assets/1cafb068-b077-46b1-8e2b-240db20eb4d5" />



# 💻<ins> Step 6 - Create A Text File On Your Local Desktop </ins>
## Open the notepad application or whichever note application is relevant to your computer.
<img width="1920" height="1029" alt="notepadScreenshot copy" src="https://github.com/user-attachments/assets/7acdc11a-af49-4ff2-955b-085d73da0935" />

## Create a text file and write a message such as, "Hello".
<img width="1920" height="1029" alt="hello-screenshot" src="https://github.com/user-attachments/assets/3c5e4d35-6ab3-4124-9e6b-eee3430496da" />


# 💻<ins> Step 7 - Upload The Text File You Created To The Azure Storage Account </ins>
## First, create a container within the storage account.
<img width="1662" height="908" alt="7 1 upload the text file new" src="https://github.com/user-attachments/assets/87f84c18-ee58-44a8-8993-f8d7b8bf5f5e" />

## Verify that the container has been created. It should look like this ⬇️.
<img width="1656" height="852" alt="7 2 container created new" src="https://github.com/user-attachments/assets/8890ad38-6965-4319-ada6-326f50861fdf" />

## Next, browse for the text file you created in Step 6 and upload it to the container.
<img width="1665" height="866" alt="7 3 upload and browse for files new" src="https://github.com/user-attachments/assets/cc79b2c5-d14e-452d-9c40-1c35eed8076c" />

## Once the text file has been uploaded, it will be visible inside the container here ⬇️.
<img width="1662" height="872" alt="7 5 continued new" src="https://github.com/user-attachments/assets/968674ed-f43f-4538-bdb3-4950e6c779d4" />



# 💻<ins> Step 8 - Edit The File Within The Storage Account (within the Azure Portal) </ins>
## Use the three-dot function next to the text file to access the drop-down menu.
## Click "View / edit" here ⬇️ to edit it within the storage account.
<img width="1906" height="862" alt="7 7 new" src="https://github.com/user-attachments/assets/393d8fc8-a670-4074-af8e-8f338748978c" />

## Edit the text file with a message such as, "Goodbye".
<img width="1790" height="813" alt="7 8 view and edit new" src="https://github.com/user-attachments/assets/af67bd89-9a54-4c01-82b8-bcd3b33ed5d9" />

## Click "Save" and move forward to Step 9.

# 💻<ins> Step 9 - Download The Text File </ins>
## Using the same three-dot function for the drop-down menu, click "Download" here ⬇️.
<img width="1899" height="882" alt="7 9 download the edited file new" src="https://github.com/user-attachments/assets/9553fcf8-c976-4878-9d75-595daf8391bc" />

# 💻<ins> Step 10 - Open The File And Observe The Changes </ins>
## Using the notepad application, observe the edit you made.
<img width="1920" height="1033" alt="10  observe new" src="https://github.com/user-attachments/assets/52539d3c-08a3-40a1-b5b0-17de5b8c37ff" />


# 💻<ins> Step 11 - Delete The Resource Group Created In Step 4 </ins>
## Go to the original resource group page. You'll find the one you've have created. Using the drop-down menu fuction, click "Delete" here ⬇️.
<img width="1642" height="824" alt="11  go to original resourse group new" src="https://github.com/user-attachments/assets/1c73126d-1a29-46ce-86e4-226958ffe328" />

## Then, enter the name of the resource group you'd like to delete and confirm the deletion.
<img width="1913" height="872" alt="11  delete resourse group new" src="https://github.com/user-attachments/assets/150e56ac-a817-400b-9d4a-195cf2ae16a2" />


## Services left running will continue to charge your subcription. The purpose of deleting resource groups is to not incur cost unnecessarily.

# 💻<ins> Step 12 - Verify That The Resource Group Has Been Deleted </ins>
## Once deleted, the resouce group page should look like this ⬇️.
<img width="1656" height="853" alt="12  Confirm deletion new" src="https://github.com/user-attachments/assets/453d9f4e-d5ea-487c-a589-40ba93bb3f8c" />

# 🎉 Congratulations
## You've reached the end of the Microsoft Azure virtual machine creation walkthrough. I hope you've enjoyed the journey and gained value as well. 



