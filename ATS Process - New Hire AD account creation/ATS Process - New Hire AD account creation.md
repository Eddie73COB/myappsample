# ATS Process - New hire – Network account creation
## Task names: AD & Email Account Setup for New Hire

|Author: Eduardo Osuna | Account: Trinity|
|-------------------------|-----------------------------------|
|Version: 1.0             |Document type: Knowledge           |
|Creation Date: 03/28/2021|Last Modification:                 |
|Owner: Eduardo Osuna    |Last modification made by:         |

<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>

### AD and Email

These kind of tasks can include three kind of requirements. 

1. Network Account creation which is the main requirement

> This Requirement is always present on this Service Request.

2. Network Account with Email address
3. Network Account with VPN Access 

> This last one might or not include Email Address as well

To have this tasks completed is needed to be sure of which path is to be chosen according with the requirements requested.

**Network Account with and Email Account**

To have a Network account only we need to have the new user created on the following path in Active Role Console:

Network account with Email Account
ARS path: Quest One ActiveRoles> Configuration > Managed Units> _Trinity > Service Desk > TRN Provision w/ Mailbox > Users

Network account without Email Account
ARS path: Quest One ActiveRoles> Configuration > Managed Units> _Trinity > Service Desk > TRN Provision w/o Mailbox > Users.

![TSM1](TSM1.png)

## Staging Steps

Follow the below steps to create the Network account. 

1. Open *Quest One Active Roles Console* and follow the path specified 
above ![TSM2](TSM2.png)

2. Click on the icon shaped as a little face (New User) to create the new user on the path specified path (you may also right click inside the folder and click *New User*) ![TSM3](TSM3.png)

3. Fill the all the fields with the user's information specified on the request. 

![TSM4](TSM4.png)

4. Click on *AB* button to generate the network user name and click on Next

![TSM5](TSM5.png)

5. Ensure there are no duplicates in the database. This can be done by checking the username (user´s name) in AD specially if it comes up with a number.

6. Create Password (First name initial uppercase + Last name initial lowercase + Employee number + If needed add zeros to comply with password length *8 characters minimum) Make sure 'User must change password at next logon' is checked.  Click next. 

![TSM6](TSM6.png)

7. Click and edit the following fields depending on the new hire request form:

![TSM7](TSM7.png)

- Enter Cost center with the configuration Physical plant number + Department number (Plant 2099 + Department 6120 > Cost Center: 209961201
- Country/Region > United States or Mexico
- edsva-trn-Provisioning Ticket Number > Enter the provisioning ticket number
- edsva-trn-VIPUser > If user is marked as VIP, select the VIP tag
- employeeNumber > Type or copy and paste user's employee number from new hire form request
- Manager > Double click on the field to be populated and then on the three dotted button, search for manager with e-mail. Click OK. (Make sure DN syntax appears in Value [see below])
    ![TSM8](TSM8.png)
    ![TSM9](TSM9.png)
- employeeType > Select *User* for all defined as direct employees and *Contractor* for all others
- o > The field *o* is destined for the business unit. To have it filled just type the number described on the new hire form request on the dropdown menu (shortcut: Type P# and press the *Down* with the your directionl path on your keyboard)
- officeLocation > Type office number from new hire form and select correct option from drop down menu.  (shortcut: Type P# and press the *Down* with the your directionl path on your keyboard)

8. 

> **Note:** The user's mailbox is created automatically depending on the path in which the new user was created.

