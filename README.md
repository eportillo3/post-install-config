<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Installation Configuration</h1>
This walkthrough involves some configuration of the open-source help desk ticketing system osTicket. This builds upon the previous project: osTicket - Prerequisites and Installation.<br />


<h2>Environments Used</h2>

- Microsoft Azure
- macOS (Host Machine)
- Windows 10
- Windows App (Remote Desktop)

<h2>Technology/Applications/Services </h2>

- osTicket
- Azure Virtual Machines




<h2>Walkthrough</h2>

</br>
<h3 align="center">
  First of all there are 2 important links:
</h3>
</br>

Admin/Analyst Login Page:
http://localhost/osTicket/scp/login.php
  
<img width="860" height="984" alt="image" src="https://github.com/user-attachments/assets/b5d4dfe4-8124-42b4-b256-c1ff5dfd38b2" />
</p>
<br />
<p>
End Users osTicket URL:
http://localhost/osTicket
  

<img width="854" height="504" alt="image" src="https://github.com/user-attachments/assets/40a2aa08-227a-442f-9543-d29cf87f8030" />
</p>
<br />
<p>
Configure Roles (for grouping permissions)<br />
Admin Panel -> Agents -> Roles<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Supreme Admin

</p>



<img width="1326" height="488" alt="image" src="https://github.com/user-attachments/assets/ad9421cc-ef27-4841-9fc5-4d979e26c0bb" />


<br />



<img width="626" height="344" alt="image" src="https://github.com/user-attachments/assets/ea1880e8-7001-419a-9bfa-e33db5c04eea" />
</p>
<br />
<p>
*Check all in Tickets, Tasks, and Knowledgebase
</p>



<img width="626" height="426" alt="image" src="https://github.com/user-attachments/assets/586d4300-ed0f-49df-a8f2-0e302d9e7e83" />

<br />




<img width="390" height="194" alt="image" src="https://github.com/user-attachments/assets/b075f511-eed8-4e83-93a2-842b7fb6258e" />
</p>
<br />
<p>
Configure Departments (Ticket Visibility, Help Desk vs SysAdmins, vs Networking)<br />
Admin Panel -> Agents -> Departments<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- SysAdmins
</p>



<img width="618" height="98" alt="image" src="https://github.com/user-attachments/assets/faa9de9a-a871-4447-80f2-0e8dc9812cc5" />

<br />




<img width="1040" height="790" alt="image" src="https://github.com/user-attachments/assets/f2ee426b-bafe-479c-ad2a-27f627d86193" />
</p>
<br />




<img width="260" height="184" alt="image" src="https://github.com/user-attachments/assets/4061fed8-9724-46ae-89cb-3df6c58698b2" />
</p>
<br />
<p>
Configure Teams<br />
Admin Panel -> Agents -> Teams (Pull Agents from different Departments)<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Online Banking

  
</p>



<img width="620" height="114" alt="image" src="https://github.com/user-attachments/assets/3d2c055a-d74f-4d62-8ef7-751332a0e1c1" />
</p>
<br />




<img width="614" height="424" alt="image" src="https://github.com/user-attachments/assets/b649574c-a454-4b53-858f-b7d27f035318" />
</p>
<br />
<p>
Allow anyone to create tickets<br />
Admin Panel -> Settings -> User Settings (UNCHECK: unregistered users can create tickets)<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Registration Required: Require registration and login to create tickets 
</p>



<img width="618" height="418" alt="image" src="https://github.com/user-attachments/assets/349d4979-0c29-46e3-b4f0-af9af0e6faa7" />
</p>
<br />
<p>
Configure Agents (workers)<br />
Admin Panel -> Agents -> Add New<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
- Jane (Dept: SysAdmins)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
- John (Dept: Support)

</p>



<img width="618" height="140" alt="image" src="https://github.com/user-attachments/assets/c5392d53-4c70-4e3d-8e0f-da7166e5ac6d" />

<br />




<img width="618" height="442" alt="image" src="https://github.com/user-attachments/assets/b50a1de5-231d-4471-b885-ec0bb1b0f165" />
</p>
<br />




<img width="574" height="250" alt="image" src="https://github.com/user-attachments/assets/d64d1b54-feb4-4b73-b65c-0711eb66bbdd" />
</p>
<br />




<img width="612" height="474" alt="image" src="https://github.com/user-attachments/assets/70997b34-1743-43dc-9b2c-54f918b1fabc" />
</p>
<br />




<img width="610" height="256" alt="image" src="https://github.com/user-attachments/assets/3b970475-c7c8-42e7-9ec3-0d1993f5d00a" />
</p>
<br />



<img width="432" height="148" alt="image" src="https://github.com/user-attachments/assets/7306bfd3-ada1-45e9-8f89-e19316de0f43" />
</p>
<br />
<p>
Configure Users (customers)<br />
Agent Panel -> Users -> Add New<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Karen
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Ken

</p>



<img width="614" height="126" alt="image" src="https://github.com/user-attachments/assets/e2bf3a35-d14d-44c4-ae83-8d7a5e1f7a3b" />
</p>
<br />
<p>
Configure SLA<br />
Admin Panel -> Manage -> SLA<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Sev-A (Grace Period: 1 hour, Schedule: 24/7)<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Sev-B (Grace Period: 4 hours, Schedule: 24/7)<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Sev-C (Grace Period: 8 hours, Business Hours)

</p>



<img width="418" height="256" alt="image" src="https://github.com/user-attachments/assets/2a79879f-4328-4e93-acc1-0f4588a64deb" />
</p>
<br />




<img width="626" height="100" alt="image" src="https://github.com/user-attachments/assets/5d87a48f-4a10-4f04-adab-fe3487634145" />
</p>
<br />




<img width="612" height="328" alt="image" src="https://github.com/user-attachments/assets/bc0bcb2e-018a-4dfc-8970-3dca278e14a7" />
</p>
<br />




<img width="618" height="406" alt="image" src="https://github.com/user-attachments/assets/971459c3-db81-4a1f-a1ad-186c73b67a27" />
</p>
<br />




<img width="612" height="394" alt="image" src="https://github.com/user-attachments/assets/a4e2c89f-4ae5-4914-8c5a-978ffb474aa2" />
</p>
<br />
<p>
Configure Help Topics (For when users create a ticket)<br />
Admin Panel -> Manage -> Help Topics<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Business Critical Outage<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Personal Computer Issues<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Equipment Request<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Password Reset<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Other
</p>



<img width="618" height="236" alt="image" src="https://github.com/user-attachments/assets/9edd592d-fb5f-4b5a-aa5c-36293909ca6e" />
</p>
<br />




<img width="614" height="322" alt="image" src="https://github.com/user-attachments/assets/fe6ca90c-ad4b-4fdc-ae9b-4203c3bb11ff" />
</p>
<br />




<img width="618" height="322" alt="image" src="https://github.com/user-attachments/assets/1bb74af1-fc91-4e7e-8bfb-313e78041e91" />
</p>
<br />
<br />
<p>
<h3 align="center">
  After this walkthrough, we now have a configuration that allows us to get started with handling user tickets.
  </h3>
</p>
