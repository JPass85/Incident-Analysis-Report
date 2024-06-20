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

 The cybersecurity team has implemented a new firewall rule to limit the reate of incoming ICMP packets and deployed an Intrusion Detection System (IDS)/Intrusion Prevention System (IPS) to filter out ICMP traffic. They have also introduced new authentication policies to prevent future attacks, including multi-fuctor authentication (MFA), a limit of three login attempts, and comprehensive employee training on safeguarding login credentials. Additionally, we plan to enhance firewall configuration and allocate resourses for acquiring a new IPS.

##

 ### Detect:

  The cybersecurity team has configured the firewall to verify source IP addresses, enabling the detection of spoofed IP addresses within incoming ICMP packets. Additionally, they have deployed network monitoring software to identify abonormal traffic patterns. To detect future unauthorized access attempts, the team will use a firwall logging tool and an IDS to monitor all incoming internet traffic.

##

### Respond:

 To prepare for future security incidents, the cybersecurity team will practively isolate affected systems to prevent further network disruption. They will then work to restore any critical systems and services impacted by the event. After restoration, the team will thorougly analyze network logs to detect any suspicious or abnormal activity. All incidents will be promptly reported to upper management, and if necessary, the team will coordinate with the appropriate legal authorities.
 
  The team has already deactivated the intern's network account and provided training sessions for interns and employees on safeguarding login credentials to prevent future incidents. Upper managment has been notified and will inform customers about the data breach via email. In addition, management is required to report the breach to law enforcement and other relevant organizations in accordandce with local regulations.

##

### Recover:

 To recover from a DDoS attack caused by ICMP flooding, it is essential to restore network services to their normal operational state. To prevent future incidents, external ICMP flood attacks can be blocked at the firewall level. To alleviate internal network congestion during an attack, temporarily suspend all non-critical network services. Prioritize the prompt restoration of critical network services. Once the ICMP packet influx has subsidee, gradually bring non-critical systems and services back online.

 The team plans to restore the deleted data by using previous night's full backup. Staff have been informed that any customer information entered or modified this morning will not be included in the backup and will need to be reentered into the database after restoration.
