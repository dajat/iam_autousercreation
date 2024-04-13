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
<img src=".png" height="80%" width="80%" alt="MS Forms Creation"/>
</p>
<p>
Loip sum.
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
<img src=".png" height="70%" width="70%" alt="Adding Parameters"/>
</p>
<p>
Loip Sum.
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
