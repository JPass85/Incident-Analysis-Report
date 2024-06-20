# Incident-Analysis-Report

### Summary:

 The company experienced a security incident where all network services suddenly ceased functioning. The cybersecurity team identified the disruption as a distributed Denial of Service (DDoS) attack, triggered by a flood of Incoming Control Message Control Protocal (ICMP) packets. They responded by blocking the attack and halting all non-critical network services to prioritize the restoration of critical ones.

 ##

 ### Incident Report

 This morning, an intern reported to the IT department that they were unable to log into their internal network account. Access logs reveal that the intern's account has been actively accessing records in the customer database, despite being locked out. The intern state that they had received an email earlier, instructing the intern to visit an external website and log in using internal network credentials to retrieve a message. We suspect this method was utilized by a malicious actor to gain unauthorized access to company network and customer database.

 Additional, serveral employees have observed that numerous customer records are either missing or contain inaccurate data. It seems that not only was customer data compromised by a malicious actor, but some data may have also been deleted or altered.

##

### Identify:

  Malicious actor(s) launched an ICMP flood attack against the company, compromising the entire internal network. This attack affected all critical network resources, which required immediate securing and restoration to ensure functionality. The inceident management team audited the implicated systems, devices, and access policies to identify security deficiencies. Their investigation revealed that the attacker had obtained an intern's login credentials, using them to access the customer database. Intitial examination indicates that some customer data may have been deleted from the database.

##

### Protect:

 
