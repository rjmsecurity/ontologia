# Active Directory

- again, AD is a centralized database to manage your users from 

- when the user logs in to the network, you can have *login scripts* run for that user
- commonly these scripts map network drives but you can make them update to the latest security software signatures and update applications

- Group Policies are the obvious thing when it comes to AD security
- you can require passwords to have a certain length and complexity
- restrict logging in to work hours and disallow accessing resources during off-hours

- AD is commonly separated into OUs (*Organizational Units*)
- commonly associated with organizational units used outside the computing environment: shipping and receiving department, marketing department
- it can be based on the different locations your organization operates in and the departments in each of those locations

- you can assign a network share on that centralized database as a user's *home folder* with all their files
- `\\server1\users\professormesser`

- *folder redirection* means the user's data is on the server and not in a local folder on the user's device
- store the Documents folder on `\\server1` and accessfiles from anywhere

#aplus #core2 **2.2** *Explain logical security concepts.* 
