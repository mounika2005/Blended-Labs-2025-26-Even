# Lab 1 - Introduction to AWS Identity and Access Management (IAM)

## Title
Introduction to AWS Identity and Access Management (IAM)


## Objective
The objective of this lab is to understand how AWS Identity and Access Management (IAM) controls authentication and authorization in AWS. The lab focuses on exploring IAM users and groups, analyzing attached policies, assigning users to appropriate groups based on organizational roles, and validating permissions by testing service access.


## Prerequisites
- Basic understanding of cloud computing concepts  
- AWS Academy Lab access  
- Web browser with internet connectivity  


## Tools Used
- AWS Management Console  
- AWS Identity and Access Management (IAM)  
- Amazon EC2  
- Amazon S3  


## Tasks Performed

### Task 1: Explore IAM Users and Groups
- Reviewed pre-created IAM users: user-1, user-2, user-3  
- Explored IAM groups: EC2-Admin, EC2-Support, S3-Support  
- Inspected managed and inline policies attached to groups  
**Screenshot:**  
<img width="1916" height="973" alt="Screenshot 2026-04-17 143141" src="https://github.com/user-attachments/assets/cd170638-04bf-43ca-8a13-724a0a15d84f" />
<img width="1911" height="972" alt="Screenshot 2026-04-17 143150" src="https://github.com/user-attachments/assets/5cce1e22-acfc-4745-8754-f87136e7e338" />
<img width="1900" height="978" alt="Screenshot 2026-04-17 143200" src="https://github.com/user-attachments/assets/ed3ab9d3-59cb-494b-a809-7e1f8e5987a1" />


### Task 2: Add Users to Groups
- Added user-1 to the S3-Support group  
- Added user-2 to the EC2-Support group  
- Added user-3 to the EC2-Admin group  
**Screenshot:**  
  <img width="1908" height="1005" alt="Screenshot 2026-04-17 142939" src="https://github.com/user-attachments/assets/8f91e6e0-dd57-4aef-bf9e-f751ab4acca1" />
<img width="1915" height="1021" alt="Screenshot 2026-04-17 143001" src="https://github.com/user-attachments/assets/03602ec0-980d-4e98-94f0-4ee0fd310cbb" />
<img width="1908" height="1005" alt="Screenshot 2026-04-17 142939" src="https://github.com/user-attachments/assets/80bccd10-b3ab-443d-a3c6-9c0beef227ac" />


### Task 3: Test IAM User Permissions
- Logged in using IAM sign-in URL  
- Verified S3 access for user-1  
- Verified EC2 read-only access for user-2  
- Verified EC2 administrative access for user-3  
**Screenshot:**  
  <img width="1916" height="1016" alt="Screenshot 2026-04-17 144950" src="https://github.com/user-attachments/assets/c79138f4-2691-4efe-896b-7ac157442574" />
<img width="1912" height="1026" alt="Screenshot 2026-04-17 144153" src="https://github.com/user-attachments/assets/e97a6d65-e954-48c3-98c1-754da29281ed" />
<img width="1907" height="1022" alt="Screenshot 2026-04-17 144022" src="https://github.com/user-attachments/assets/8134f124-6631-4b13-ba1b-b119327c5fa1" />



## Workflow
1. Accessed IAM console and reviewed users and groups.  
2. Inspected policy permissions attached to groups.  
3. Assigned users to groups based on their roles.  
4. Logged in as each IAM user using the sign-in URL.  
5. Validated permissions by accessing AWS services.  


## Learning Outcomes
- Understood the role of IAM in AWS security.  
- Learned how IAM users, groups, and policies interact.  
- Gained practical experience implementing role-based access control.  
- Verified permission enforcement through real-time service testing.  


## Conclusion
This lab provided hands-on experience with AWS IAM by demonstrating how organizations manage secure access to cloud resources. Assigning users to groups with predefined policies simplified permission management and ensured role-based access control across AWS services.


## Author
**Name:** levaku lakshmi mounika-212223100026
**Course:** Introduction to Cloud Computing  

