#  Salesforce SOAP API Login Task

This repository contains my completed task of successfully logging into Salesforce using the **SOAP API** via **SOAP UI**.

---

##  Objective

The goal of this task was to:
- Perform a SOAP-based login to Salesforce
- Understand how to use the Salesforce `sessionId` and `serverUrl`
- Save both the request and response XML files
- Mask sensitive credentials for public sharing

---

##  Tools Used

-  **SOAP UI** (for testing the SOAP login)
-  **Salesforce Developer Edition** (for credentials and endpoint)
-  **GitHub** (to host the XML files)

---

##  Files Included

| File Name            | Description                                           |
|---------------------|-------------------------------------------------------|
| `login-request.xml` | SOAP request XML used to log in (credentials masked) |
| `login-response.xml`| SOAP response from Salesforce (session ID masked)    |

---

##  Sample SOAP Login Request

```xml
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/"
   xmlns:urn="urn:partner.soap.sforce.com">
   <soapenv:Header/>
   <soapenv:Body>
      <urn:login>
         <urn:username>your_username@example.com</urn:username>
         <urn:password>yourPasswordMASKEDSecurityToken</urn:password>
      </urn:login>
   </soapenv:Body>
</soapenv:Envelope>
