Developer: External entity who is a user of the system. He/She can upload software to find the license and vulnerabilities.
Manager: External entity who overlooks the system.  This user can get project information, policy information and make changes to the policy.
National Vulnerability Database: External database that stores the most up to date known vulnerabilities based off of software licensing.
Manage Software Information: A system process that takes user inputted software and finds the licenses and known software vulnerabilities and stores them in the system database.
Scanner: A system process that takes the user inputted software and determines the licenses associated with it.
Manage Project Information: A system process that communicates with the Manager and the CPE software information database to send the manager project information.  This process also checks the policy and sends the manager results.
Send Software: A data flow Initiated when user uploads software to end up in the scanner where it can process what software licenses are present.
License Results: A Data flow that is a scanner response to send software that gives the licenses of the software.  This is sent back to the developer, the software database and the vulnerability database.
Vulnerability Results: A data flow that is a response from the Vulnerability Database in response to the license results.  This data flow contains the vulnerabilites of the software and sends them to the developer and the software information database.
Results: A data flow that represents the license and vulnerability results that are sent back to the developer from the scanner and the vulnerability database.
Vulnerabilty Request: A data flow request made by the system process manage vulnerability information that asks the national vulnerability database to send up to date license vulnerabilities.
Vulnerability Responce: A data flow response from the national vulnerabilty database giving the CPE vulnerabilty database the most up to date license vulnerabiltiy information.
Project Info Request: A data flow request made by the manager to get project information from the software information database.
Project Info Response: A data flow response from the software information database back to the manager that contains the software license and vulnerabilities.
Check Policy: A data flow Response from the system process manage project information that checks the software licenses with company policy to make sure that they are acceptable.
Policy Response: A data flow response from the CPE company policy database back the the system process manage project information to send to the manager with the results of any policy violations.
Update Policy: A data flow representing the managers authority to modify company policies pertaining to software licenses and vulnerabilities.
