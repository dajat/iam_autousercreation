<p align="center">
<img src="https://imgur.com/i4tvZYY.png" height="50%" width="50% alt=" Microsoft Entra"/>
</p>

<h1>Automated User Creation (Azure)</h1>
This tutorial outlines creating an MS Entra ID group and adding a dynamic query to create a user attribute to assign the user to the appropriate MS Entra ID group. This tutorial will outline how to use a Microsoft Form to trigger and automate a workflow built in Power Automate to create user profiles inside of Microsoft Entra ID. Please ensure that the following subscriptions are active:

- Entra ID Premium P2
- Microsoft Business Basics

Both of these subscriptions can be used as free trials for one month.
<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Microsoft Entra ID)
- Microsoft Forms
- Microsoft Power Automate

<h2>Installation Steps</h2>

<h2>Creating a Group in Microsoft Entra ID</h2>
<p>
<img src="https://imgur.com/5vE8Y1I.png" height="60%" width="60%" alt="Microsoft Entra Group"/>
<img src="https://imgur.com/coTeftQ.png" height="50%" width="50%" alt="Microsoft Entra Group"/>
</p>
<p>
Select Microsoft Entra ID > Groups > New Group > Select Group type, and add Group name and membership type. Select security as the group type, select dynamic user for the membership type, and name the group help desk for this project. Select Dynamic User for membership type to have a specific administrator to control membership access and rules. The rules for the membership allow the administrator to add an attribute to define members and add them to a group. Next, select 'No members selected' to add the dynamic query.
</p>
<br />
<h2>Adding an Attribute-Based Access Control (ABAC) query</h2>
<p>
<img src="https://imgur.com/Z8fHMOn.png" height="60%" width="60% alt="ABAC query"/>
<img src="https://imgur.com/GCBv52G.png" height="60%" width="60% alt="ABAC query"/>
</p>
<p>
For the dynamic membership rule, select ‘Department’ under ‘Choose Property’, choose ‘Equals’ for Operator, and add ‘Help desk’ as the Value > Select Save. After a few seconds, you will see that the ‘Help Desk’ group appears under ‘All Groups’.
</p>
<br />
<h2>Creating a Form in MS Forms</h2>
<p>
<img src="https://imgur.com/52zp8NH.png" height="80%" width="80%" alt="MS Forms Creation"/>
</p>
<p>
Create a form in MS Forms > Select New Form, once you are signed into their MS Forms account. This is the starting point of the project and where we begin to build out the steps for automating the joiner process.
</p>
<br />
<h2>Creating a Workflow in Power Automate</h2>
<p>
<img src=".png" height="70%" width="70%" alt="Power Automate Workflows"/>
</p>
<p>
Loip sum.
</p>
<br />
<h2>Adding Parameters for each Action Workflow</h2>
<p>
<img src="https://imgur.com/jXO30Q9.png" height="70%" width="70%" alt="Adding Parameters"/>
<img src="https://imgur.com/mDhIhhv.png" height="70%" width="70%" alt="Adding Parameters"/>
</p>
<p>
Open MS Power Automate > My Flows > New Flow (you can create from a blank canvas or a template) > Select automated cloud flow under build from a blank canvas. Create flow, add the flow name, and choose ‘When a new response is submitted’ from the flow triggers. Select the flow that was created and select the form that was created previously. Next, select the plus icon and ‘Add an action’. Select the Microsoft Forms tab and select the trigger ‘Get response details. *It should ask you to ‘Sign In’ to connect to Microsoft Forms.*
</p>
<br />
<h2>Adding Parameters for each Action Workflow Continued</h2>
<p>
<img src="https://imgur.com/1QRQFAP.png" height="70%" width="70%" alt="Adding Parameters"/>
</p>
<p>
After signing in, you will select the Onboarding form as the Form ID and enter a unique identifier for the Response ID by selecting the lightning bolt to the right. Next, we will do the same for the next action by selecting Create a user from Microsoft Entra ID.
</p>
<br />
<h2>Adding Parameters for each Action Workflow Continued</h2>
<p>
<img src="https://imgur.com/9MuH0AU.png" height="70%" width="70%" alt="Adding Parameters"/>
<img src="https://imgur.com/UI4pqZW.png" height="70%" width="70%" alt="Adding Parameters"/>
<img src="https://imgur.com/yLxnP5x.png" height="70%" width="70%" alt="Adding Parameters"/>
</p>
<p>
In the search bar, you can search for 'Entra' and select 'Create A User'. Next, you will fill in the parameters by selecting the lightening bolt to the right to fill in the information that is connected from the Microsoft Form that was created earlier.
</p>
<br />
<h2>Testing the Work Flow</h2>
<p>
<img src=".png" height="70%" width="70%" alt="Automation Testing"/>
</p>
<p>
Loip Sum.
</p>
<br />
