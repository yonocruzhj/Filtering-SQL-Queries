<h1>Apply Filters to SQL Queries</h1>

<h2>Description</h2>
Project consists of a simulation to perform security-related tasks using filtering methods via SQL. Tasks include updating employee computers as needed and investigating potential security issues through failed logins and other suspicous activity.
<br />


<h2>Languages and Utilities Used</h2>

- <b>SQL</b>
- <b>Bash shell</b>

<h2>Tasks:</h2>

<p align="center">
Scenario: <br/>
The company asked me to look into potential security incidents and update computers. My first task was to investigate failed login attempts at a suspocious operating time (18:00). My second task was to investigate login attempts on specific dates '2022-05-09' and '2022-05-08'. The third task was to retrieve login attempts outside of Mexico. Finally, my last task was to update computers outside the IT department. 
<br />
<br />
Retrieve after hours failed login attempts:  <br/>
<img src="https://imgur.com/0Eh5rxf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
The first portion is the code I used to filter failed login attempts after 18:00. The first condition **login_time > '18:00'** filters for logins only after 18:00 and the second condition **success = FALSE ** filtered for failed login attempts. The second portion is the output generated.
<br />
 
Results were 19 after hours failed login attempts : <br/>
<img src="https://imgur.com/RE18oDf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
 
<br />
Retrieve login attempts on specific dates:  <br/>
<img src="https://imgur.com/GYS9NBG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
 The first portion is the code I used to filter for login attempts on the dates **'2022-05-09** and **'2022-05-08**. 
<br />


<br /> 75 login attempts on these 2 dates:  <br/>
<img src="https://imgur.com/TboZ5DJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />


<br />
Retrieve login attempts outside of Mexico  <br/>
<img src="https://imgur.com/BFcMuuP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
The team narrowed the search down by filtering login attempts outside of Mexico. The first portion is the code I used to filter for login attempts that were not from Mexico. The second portion is the output.
<br />

<br /> 144 login attempts outside of Mexico<br/>
<img src="https://imgur.com/Ip50XzN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br /> 


Retrieve employee information not in IT<br />
<img src="https://imgur.com/SCtY5eQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
As for the task of updating computers in the company's different departments. All computers required an update besides the IT department, so I retrieved all employee information outside of IT using the code listed above.
<br />

Updates needed in other departments excluding IT  <br/>
<img src="https://imgur.com/lBiR5gx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

<h2>Summary</h2>
I filtered SQL queries to obtain needed information and to investigate login attempts and employee machines. For the login attempts I used the table **log_in_attempts** and for the employee information I used **employees**. I used various operators to filter information and complete my tasks based on the scenario. 

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
