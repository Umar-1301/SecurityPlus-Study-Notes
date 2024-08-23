### Authentication and Access Controls

# Introduction


There are 4 main categories of controls: - Technical - Admin - Physical - Operational
Simple definition of Control is to safeguard assets, protect sensitive information, meet business security objectives, and prevent security breaches
With that said controls belong to one or many categories, serving different aspects of an organisation

Technical - Technology based controls to safeguard assets on the network - Firewall, Antivirus, IDS
Admin - An organisations policies and procedures -  Passwords, MFA, Policies
Physical - The physical security of critical infrastructure where physical access can cause harm - Cameras, Gates, Doors
Operational - Concerning the day to day operation, tasks being performed, users on the network - Training, Education

From here you can look at the types of controls that can be in any of these categories. The types are as follow:
* Detective - A control that detects issues - during - IDS, Cameras, Reports
* Corrective - Corects the detected issue - after - Patches, IRP, Policy changes
* Detterant - Detters the issue from occuring - Before - Warnings, Training, Procedures
* Compensating - If an attack was to happen, this control should be in place as compensation - during/after - backup data, switching network
* Preventive - Prevents issues from even occuring - Before - Fire Walls, Encryption, Layered Defence and....

# Access Controls

Access control = Preventing or granting access which is done by Identificiation, Authentication and Authorisation
some examples:

MAC ( mandatory access controls ) - Policy driven and non-flexible, decided by admin or security officers, used for highly secure data such as patient information
DAC ( discretionary access control ) - Flexible access, determined by resource owner, such as a windows or linux file permissions, used for business documents that arent deemed sensitive but still should be secured
RBAC ( role based access control ) - Access determined by users roles within an orginastion, call handler may have access to basic patient data but doctors will have permissions to see entire medical history
ABAC ( attribute based access control ) - Based on attributes rather than just role, for example department and location, you cannot access example.file if you are out of site, time of day, data sensitivity
GBAC ( group based access control ) - Granting or denying access to groups, departments, job function, project team




