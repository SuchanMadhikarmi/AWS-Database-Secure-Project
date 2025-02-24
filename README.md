<h1>Cloud Security Project: Securing an AWS RDS Database</h1>



<h2>Description</h2>
This project focuses on understanding and mitigating security vulnerabilities in AWS RDS (Relational Database Service). The primary objective was to simulate and identify insecure configurations, perform SQL injection attacks, and implement best practices to secure the database. The project covers essential security tasks such as modifying security groups, enforcing strong authentication, and enhancing access controls.<br/>


<br />

<h2>Tools and Technologies Used</h2>

- <b>AWS Services: RDS, EC2, CloudTrail, CloudWatch
- <b>Database: MySQL (or PostgreSQL, as applicable)
- <b>Command-Line Interface: Windows CMD/Terminal
- <b>Security Concepts: Network ACLs, Security Groups, Encryption, SQL Injection

<h2>Key Features</h2>
- Simulated an insecure AWS RDS database setup<br/>
- Performed SQL injection to exploit vulnerabilities.<br/>
- Implemented security measures: strong passwords, restricted public access, and backups.<br/>
- Configured Network ACLs and Security Groups for fine-grained access control.<br/>
- Created database snapshots for disaster recovery.<br/>
- <br/>


<h2>Steps Undertaken :</h2>

  1. <b>Setting Up an Insecure AWS RDS Database</b><br/>
     - Created an RDS MySQL instance with public access enabled.<br/>
     - Created a new Security Group and allowed all inbound traffic (0.0.0.0/0) for testing purposes.<br/>
     </br>
    

     <img src="https://i.imgur.com/5XLkCmK.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
     <img src="https://i.imgur.com/y2yfijZ.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
     <img src="https://i.imgur.com/rMFKLj3.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
     <img src="https://i.imgur.com/ydRz6SE.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
     
<br />
<br />
 2. <b>Accessing the Database via Command Prompt</b><br/>
       - Used the RDS endpoint to connect to the database:<br/>
       - Verified successful remote access with public exposure.<br/>
       - Created a table and added valeus.<br/>
         <br/>
  

<img src="https://i.imgur.com/olpeKov.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/FGmWLAk.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
<br />
<br />

  3. <b>Simulating SQL Injection</b><br/>
      - Executed a basic SQL injection:<br/>
      - Verified that the injection successfully bypassed authentication.<br/>
        <br/>

<img src="https://i.imgur.com/qeJ2G0q.png" height="90%" width="80%" alt="Disk Sanitization Steps"/>

<br />
<br />
 4. <b>Securing the AWS RDS Instance</b><br/>
       - Enforced strong password policies (e.g., minimum length, special characters).<br/>
       - Allowed inbound access only from specific IP addresses<br/>
       - Removed the open access (0.0.0.0/0) rule.<br/>
       - Disabled Public Access:<br/>
       <br/>
       
     
<img src="https://i.imgur.com/76UqDf7.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/M09Kcss.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/aC7R2rm.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>

<br />
5. <b>Enhancing Backup and Disaster Recovery</b><br/>
       - Created an RDS snapshot for point-in-time recovery.<br/>
       - Changed backup retention period to ensure regular backups <br/>

  <br/>
<img src="https://i.imgur.com/aGNJ5sA.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>

<br />

5. <b> Configuring Network ACLs</b><br/>
       - Edited Network ACL to restrict inbound and outbound database traffic to necessary ports<br/>

  <br/>
<img src="https://i.imgur.com/jX3EYbj.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>

<br />




<h2>Key Learnings</h2>
     -Understood AWS RDS configurations and their impact on database security.<br/>
     - Simulated and mitigated SQL injection vulnerabilities.<br/>
     - Implemented industry best practices for securing cloud databases.<br/>
     - Learned to manage access control using AWS Security Groups and Network ACLs.<br/>


</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
