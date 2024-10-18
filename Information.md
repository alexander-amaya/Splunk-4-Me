# Tasks
## Task 1: IT Operations: Investigate successful versus unsuccessful web server requests over time

<br></br>

Being tasked to investigate successful versus unsuccessful web server requests over time. I used the input shown on the image to successfully collect all data that matched the input. 
![image](https://github.com/user-attachments/assets/7402cef1-de22-4df6-8b1a-66d258c3cf1e)

After a successful search, we need to make sense of the data. We are tasked with creating a visualization to help better digest the information. We will press the "Visualization" button to show us how we'd like to configure our image. We will do this with a column chart. We will then properly save this by creating a dashboard for us to place the results of all of our tasks. 

![image](https://github.com/user-attachments/assets/f59e8b3c-d7a8-4c3a-824c-7485f610c1b6)
This is our result.

<br></br>

## Task 2: DevOps: Show the most common customer operating systems and which web browsers are experiencing the most failures

<br></br>

We are tasked with filtering the most common operating systems our customers use and which web browsers are experiencing the most failures. To successfully find this data, we will need to create a New Field. Splunk populates certain fields while others need to be created. We will be creating a "Platform" field to be able to determine the operating systems and the web browsers that the customers use. 

To create a New Field we will begin by selecting the down arrow on an event. 

![image](https://github.com/user-attachments/assets/b7b53276-e75b-44cb-b108-1bd4217071de)

We will then select "Event Actions" followed by "Extract Fields"

![image](https://github.com/user-attachments/assets/2fca8def-1dda-4a27-8868-8781360bffc5)

We will be prompted with a new screen that will indicate that we are ready to define what the new field will be. Once on the new screen, you will select the "Regular Expression" button. Followed by "Next" near the top. 
![image](https://github.com/user-attachments/assets/bdcf21d3-627c-492d-81bd-1ceb70c0819f)

This will then take us to a new page where we will define what the new field will be. We will highlight the part of the event that is of interest and give it a new name.

![Screenshot22222222](https://github.com/user-attachments/assets/60c86d81-e2ee-4cd1-9c78-df0be0f5b37e)

With this newly defined field, we can extract the data and filter it to show us which operating systems are most common and which web browsers are experiencing the most failures. We will go back to our data. In the Events section, on the left-hand side, we will see our newly generated field "platform" appear. We will select that displaying the 4 platforms that are used to visit the site. We will then select "Top Values" to exclusively filter out this data only. The final result should appear as shown below.

![image](https://github.com/user-attachments/assets/b643b40b-e259-4d5a-bb85-9051a2f62de8)

Now, we can add this to our existing dashboard where we have already added the visualization from task 1. 

We must now filter out the web browsers that are experiencing the most failures. We will use this command to show us what web browsers fail the most. 

![image](https://github.com/user-attachments/assets/7aa5cf81-8294-4f66-8f69-2af1ae460a83)

As we complete this step, we will not have 3 panels on our dashboard. You can edit and rearrange your dashboard however you'd like with the "Edit" button on the upper right-hand side. When you are done configuring your dashboard, it should look like this. 

![image](https://github.com/user-attachments/assets/da166af1-5036-46c1-a35f-2b609589123e)


<br></br>

## Task 3: Business Analytics Team: Show the lost revenue from the website

<br></br>

We are now being tasked with showing all lost revenue from the website. We first need to make sure that there is a file that makes sure there is a "product_price" filter. We do this by verifying it with the "Lookups" feature. It will be under the "Settings" tab as shown below.

![image](https://github.com/user-attachments/assets/6e06e8b3-7af8-4c72-a0b9-125014239333)

Once we click "Lookups" we will clock on "Lookup table files." We want to make sure that this file is shown because this is the file which we will get our product_price from.

![image](https://github.com/user-attachments/assets/d552499a-a638-45fd-a714-38f81924a134)

We can now begin to complete the task that the Business Analytics team is asking for. We will start by searching through the data with this command. This command retrieves additional fields from the lookup file that may not have been shown to us before as this command allows us to narrow it down to a specific file. 

![image](https://github.com/user-attachments/assets/03992011-ff46-4865-8b1c-df94b0d652c7)

We know the command works because we can see a "product_price" filter now appear on the left-hand side. From there we will now be more specific and write a new command. This command will filter out the lost revenue from the website and show us how much that equates to dollars.

![image](https://github.com/user-attachments/assets/06eb7628-0d30-4d5c-83bf-ba41b9f73650)

Once the data populates, you are now able to visualize it. You will begin by clicking the "Vizaulation" button then "Single Value" and finally the "Single Value" button to show us a single number value.

![image](https://github.com/user-attachments/assets/4af763e8-f8c6-493f-bc6b-6dfbad9e8834)

Your dashboard should look like this now.


![image](https://github.com/user-attachments/assets/a3ef9e3a-c6d1-4fd2-ab1e-dbf3d7ddc36e)
*Disclaimer* when I initially did this project there was a number value there of $36.25 but as I try to do this again later in the day it appears as N/A. I am not sure why and have tried multiple times to correct this but with no luck. Yours should have a number value if working properly. 

<br></br>

## Task 4:Security and Fraud Team: Show website activity by geographic location

<br></br>

We are not being tasked by the Security and Fraud team to show activity by geographic location. To retrieve this information we will be using two new commands to help us, "iplocation" and "geostats". The entire command will look like this as we look to narrow the data by city.

![image](https://github.com/user-attachments/assets/42f47521-08c6-47a2-834f-0a095e6ee38d)

After running the command, you will select the "Visualization" tab to generate readable information. It will look like this.


![image](https://github.com/user-attachments/assets/5deaf59a-0d88-4673-bef8-f27994105732)

From there, you will select "Save As" and add it to our existing dashboard as we have done for all other tasks.  

Your new and completed dashboard should look like this.

![image](https://github.com/user-attachments/assets/df41277b-9775-4e0d-a225-9dc7a4d887ef)

We have now completed all the tasks that each team has requested of us. We can now demonstrate with appealing visuals all the information that is important to each team. 
