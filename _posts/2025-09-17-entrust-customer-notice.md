---
layout: article
title:  "Entrust Customer Notice: New SSL CA Root Certificate must be imported in Identity Enterprise Self-Service Module (SSM) Key Store."
header:
  teaser: /assets/images/2025-09-17-entrust-customer-notice.jpg
categories:
tags:
date: 2025-09-17
updated_date: 
---
![image tooltip here](/assets/images/2025-09-17-entrust-customer-notice.jpg)

Attention Entrust Identity Enterprise Customers,

We wish to inform you that the SSL certificate used by the Entrust Identity Notification Service will be updated. The new certificate will be issued by an alternate Certificate Authority —Sectigo.  

After the SSL certificate update is done, push notifications from your Identity Enterprise Self-Service Module (SSM) to your mobile end users will fail unless the Sectigo Root CA certificate is added to your SSM Key Store. 

Effective Date of Change
The SSL certificate update for the Entrust Identity Notification Service will take effect on October 16, 2025.

Who is Affected and Impacts
The upcoming SSL certificate change for the Entrust Identity Notification Service will affect Entrust Identity Enterprise customers who use SSM to send mobile push notifications to their end users. 
 
If the issued Sectigo Root CA certificate is not added to the SSM Key Store configuration before October 16, 2025,end users will not receive push notifications for time sensitive authentication and transaction verification. 
 
Your Identity Enterprise SSM Administrators will observe the following error text in the Self-Service transaction log: javax.net.ssl.SSLPeerUnverifiedException: peer not authenticated.

Mitigation Impacts
To continue sending push notifications to mobile app users, youmust import the specified Sectigo Root CA certificate into your SSM Key Store before October 16, 2025. It is important to note that the SSL Entrust CA root certificate currently saved in your SSM Key Store must not be removed prior to October 16th cutover.  
 
Please carefully review and follow the technical procedures outlined in the documentation published in TrustedCare https://trustedcare.entrust.com/ and download the required SSL CA Root Certificate at: Products ➔ Identity ➔ Identity Enterprise ➔ Self-Service Module 13.0 ➔ Patches tab ➔ “Identity Enterprise Self-Service Module – SSL certificate for notify.entrust.com”  and click on the “View Patch Details ” option. 

Support
If you have any questions or concerns with regard to the above SSL CA root certificate replacement, please contact Entrust Customer Support. The support phone numbers can be found at: https://www.entrust.com/contact-support. 
 
Alternatively, please send an e-mail to Support Team. 

Thank you,
Entrust