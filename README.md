<h1>Applying more filters in SQL </h1>



<h2>Description</h2>
In this lab, I applied more filters to SQL queries to retrieve information from a database. I used common operators in SQL to filter by specific dates and times. I used the MariaDB shell to run your SQL queries.
<br />


<h2>Practical experience gained in this Lab</h2>

- <b>The WHERE keyword</b> 
- <b>The BETWEEN and AND operators</b>
- <b>Operators for working with numeric or date and time data types</b> 


<h2>Environments Used </h2>

- <b>Qwiklabs</b> 

<h2>Lab walk-through:</h2>

<h2>Task 1: Retrieve login attempts after a certain date </h2>
In this task, I investigated a recent security incident. To do this, I need to gather information about login attempts made after a certain date. 
<br /> <br />
(1) First, I used the command "SELECT * FROM login_in_attempts WHERE login_date > '2022-05-09';" to retrieve data for login attempts made after '2022-05'09'. 
<br /> <br /> <p align="center">
<img src="https://imgur.com/qwiDK0t.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br /> <br />
Now, I expanded the date range to include 2022-05-09 in your search.
<br /> <br />
(2) Finally, I used the command "SELECT * FROM login_in_attempts WHERE login_date >= '2022-05-09';" to retrieve data for login attempts that were made on or after '2022-05-09'.  
<br/> <br/> <p align="center">
<img src="https://imgur.com/VdLIaLM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br /> <br />

<h2>Task 2: Retrieve logins in a date range </h2>
In this task, I narrowed the focus of the search. 
<br/> <br />
(1) I used the command "SELECT * FROM login_in_attempts WHERE login_date BETWEEN '2022-05-09' AND '2022-05-11';" to retrieve the required records. 
<br /> <br /> <p align="center">
<img src="https://imgur.com/YQAppbG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br /> <br />

<h2>Task 3: Investigate logins at certain times </h2>
In this task, I investigated logins that were made at certain times. My organization's typical work hours begin at 07:00:00. 
<br/> <br/>
(1) First, I used the command "SELECT * FROM login_in_attempts WHERE login_time < '07:00:00';" to retrieve data for login attempts made before '07:00:00'.  
<br/> <br/> <p align="center">
<img src="https://imgur.com/n5Yvvsp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br /> <br />
(2) Finally, I used the command "SELECT * FROM login_in_attempts WHERE login_time BETWEEN '06:00:00' AND '07:00:00';" to return logins between '06:00:00' and '07:00:00'.  
<br/> <br/> <p align="center">
<img src="https://imgur.com/VtMVJjz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br /> <br />

<h2>Task 4: Investigate logins by event ID </h2>
In this task, I investigated login attempts based on event ID numbers.
 <br/> <br/> 
(1) First, I used the command "SELECT event_id, username, login_date FROM login_in_attempts WHERE event_id >= 100;" to return login attempts with event_id greater than or equa to 100. <br/>
<br/> <br/>  <p align="center">
<img src="https://imgur.com/xA9EYza.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br /> <br />
(2) Finally, I used the command "SELECT event_id, username, login_date FROM login_in_attempts WHERE event_id BETWEEN 100 and 150;" to return only login attempts with event_id between 100 and 150. 
<br/> <br/>  <p align="center">
<img src="https://imgur.com/dA3p7H7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br /> <br />
