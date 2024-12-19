---
title: CKLS Technical Prerequisites
keywords: pre-requisites, prerequisites, requirements
last_updated: 20 February, 2024
sidebar: home_sidebar
permalink: CKLS-prerequisites
folder: prerequisites
---

<div class="alert alert-warning" role="alert">
    <h2>Requirements for use</h2>
    <h3>Unique email address for Program Builder Early Adoption and new reporting services</h3>
    Requirements for Program Builder Early Adoption and new reporting services:  all users (administrators and learners), will need to have <b>a unique email address</b> to access the Program Builder Early Adopter and New Reporting Service.
</div>


## Workstation requirements

CrossKnowledge Learning Suite is a web-based application needing the following environment to run properly:

Screen resolution|1024*768
Sound card|Recommended (speakers/headphones are required for most content)
RAM|4GB+
Operating system|Microsoft Windows 10+, latest macOS version of Apple
Web browser|Microsoft Edge (latest version), Apple Safari (latest version), Google Chrome (latest version), Mozilla Firefox (latest version)
Email clients|Standard email readers are supported to deliver CK standard emails. Email content is HTML.
Popup blocker|Disabled
Cookies|Enabled
JavaScript|Enabled
HTTPS|SSL Protocol: TLSv1.2<br>SSL Ciphers:<br>- ECDHE-ECDSA-AES128-GCM-SHA256<br>- ECDHE-RSA-AES128-GCM-SHA256<br>- ECDHE-ECDSA-AES128-SHA256<br>- ECDHE-RSA-AES128-SHA256<br>- ECDHE-ECDSA-AES128-SHA<br>- ECDHE-RSA-AES128-SHA<br>- ECDHE-ECDSA-AES256-GCM-SHA384<br>- ECDHE-RSA-AES256-GCM-SHA384<br>- ECDHE-ECDSA-AES256-SHA384<br>- ECDHE-RSA-AES256-SHA384<br>- ECDHE-RSA-AES256-SHA<br>- ECDHE-ECDSA-AES256-SHA<br>- AES128-GCM-SHA256<br>- AES128-SHA256<br>- AES128-SHA<br>- AES256-GCM-SHA384<br>- AES256-SHA256<br>- AES256-SHA<br>

<br>
We systematically test the latest versions of Chrome, Firefox and Edge browsers to ensure the best experience for our users. Older versions of these browsers are not systematically tested, but run smoothly in most cases. If, however, there is a problem specific to a particular version of one of these browsers, please contact us.

These technical requirements may be modified according to technical developments of CrossKnowledge solutions.
In addition to those, specific requirements apply to:
- Blendedˣ Embedded Web Resource Activity and Embedded BI tool in Analyze workspace: these features are used to integrate a 3rd party content from the web. CrossKnowledge can not guaranty the compatibility of the integrated content

In order to ensure a good user experience for Blendedˣ Embedded Content Activity, please ensure that SCORM content are built to be responsive.


### Tablet compatibility

CrossKnowledge Learning Suite is compatible with iPad (latest version) - additional requirements may be needed for the content hosted on the Learning Suite.

CrossKnowledge Learning Suite is compatible with Android tablets (Chrome browser) - additional requirements may be needed for the content hosted on the Learning Suite.

Please note that SCORM and AICC connectors are not optimized for mobile usage.

### CrossKnowledge content additional requirements

As the content are played on our Learning Suite, you need the Learning Suite requirements listed above, and the following ones:

<table width="100%">
    <tbody>
        <tr>
            <td width="45%">PDF plugin</td>
            <td width="55%">Adobe Acrobat Reader DC (latest version)</td>
        </tr>
    </tbody>
</table>


## Network Information

### Media extensions
The following media extensions should be authorised.<br/>
`.mp3, .mp4, .srt, .woff, .vtt, .xhtml`

### SFTP access
Customers should provide CrossKnowledge with a valid public key for access to be granted on CrossKnowledge SFTP servers.

SSH keys should follow the following rules:
- Use 4096 bits;
- Should be renewed once a year on customer request.

### Domain white-listing
The following domain names should be whitelisted by customers and their partners.
```txt
https://*.crossknowledge.com, https://*.crossknowledge-china.com, https://*.learnosity.com​, https://s3.amazonaws.com/assets.learnosity.com, https://s3.amazonaws.com/learnositymediaprocessed, https://*.powerbi.com, https://content.powerapps.com, https://wabi-us-east2-d-primary-redirect.analysis.windows.net
```

If wildcards (*) are not allowed, authorise the following sub-domains:<br/>

```txt
https://ace-static.crossknowledge.com
https://cdn-cklm-prod.crossknowledge.com
https://ckcg.crossknowledge.com
https://ckconnect-static.crossknowledge.com
https://ckconnect.crossknowledge.com
https://ckls-api.crossknowledge.com
https://ckls-assets.asia.crossknowledge.com (Only for CKLS hosted in Japan)
https://ckls-assets.eu.crossknowledge.com (Only for CKLS hosted in Europe)
https://ckls-assets.na.crossknowledge.com (Only for CKLS hosted in USA)
https://ckls-assets.sa.crossknowledge.com (Only for CKLS hosted in Brazil)
https://ckls-assets.ckls.crossknowledge-china.com (Only for China dedicated CKLS)
https://ckls-cdn.crossknowledge-china.com
https://ckls-cdn.crossknowledge.com
https://d12pbbvc3h54xm.cloudfront.net
https://d3d8qnlcu0b7xk.cloudfront.net
https://media.crossknowledge.com
https://media-cdn2.crossknowledge.com
https://spa.crossknowledge.com
https://api.crossknowledge.com
https://api.crossknowledge-china.com
https://app-cdn.crossknowledge.com

Learnosity specific URLs

https://authorapi.learnosity.com
https://items.learnosity.com
https://items-va.learnosity.com
https://items-au.learnosity.com
https://items-ie.learnosity.com
https://items-ca.learnosity.com
https://reports.learnosity.com
https://reports-va.learnosity.com
https://reports-au.learnosity.com
https://reports-ie.learnosity.com
https://reports-ca.learnosity.com
https://data.learnosity.com
https://data-va.learnosity.com
https://data-au.learnosity.com
https://data-ie.learnosity.com
https://data-ca.learnosity.com
https://annotations.learnosity.com
https://annotations-va.learnosity.com
https://annotations-au.learnosity.com
https://annotations-ie.learnosity.com
https://annotations-ca.learnosity.com
https://assess.learnosity.com
https://assess-va.learnosity.com
https://assess-au.learnosity.com
https://assess-ie.learnosity.com
https://assess-ca.learnosity.com
https://eventbus.learnosity.com
https://eventbus-va.learnosity.com
https://eventbus-au.learnosity.com
https://eventbus-ie.learnosity.com
https://eventbus-ca.learnosity.com
https://events.learnosity.com
https://events-va.learnosity.com
https://events-au.learnosity.com
https://events-ie.learnosity.com
https://events-ca.learnosity.com
https://questions.learnosity.com
https://questions-va.learnosity.com
https://questions-au.learnosity.com
https://questions-ie.learnosity.com
https://questions-ca.learnosity.com
https://questioneditor.learnosity.com
https://questioneditor-va.learnosity.com
https://questioneditor-au.learnosity.com
https://questioneditor-ie.learnosity.com
https://questioneditor-ca.learnosity.com
https://schemas.learnosity.com
https://schemas-va.learnosity.com
https://schemas-au.learnosity.com
https://schemas-ie.learnosity.com
https://schemas-ca.learnosity.com
https://assets.learnosity.com
https://shared.learnosity.com
https://s3.amazonaws.com/assets.learnosity.com
https://s3.amazonaws.com/learnositymediaprocessed

Power BI specific URLs

https://appsource.powerbi.com
https://app.powerbi.com
https://content.powerapps.com
https://wabi-us-east2-d-primary-redirect.analysis.windows.net
https://pbivisuals.powerbi.com
```

### CloudFlare IP Ranges
All requests to CKLS URLs are going through CloudFlare Network.
Please follow this link to find [CloudFlare IP ranges](https://www.cloudflare.com/fr-fr/ips/)

### CKLS portal IP addresses

#### Europe CKLS https://*.eu.crossknowledge.com:
```txt
sftp server : sftp-aws.eu.crossknowledge.com (52.58.183.197)
```

<br/>

#### USA https://*.na.crossknowledge.com:
```txt
sftp server : sftp.na.crossknowledge.com (54.221.219.193)
```

<br/>

#### South America: https://*.sa.crossknowledge.com
```txt
sftp server : sftp.sa.crossknowledge.com (54.232.80.112)
```

<br/>

#### Asia: https://*.asia.crossknowledge.com
```txt
sftp server : sftp.asia.crossknowledge.com (54.65.104.30)
```

<br/>

#### IPs addresses and URLs for CK-Hub https://ck-hub.crossknowledge.com:
```txt
web interfaces (ports 80 and 443) : Could be hitting any of the eu-west-1 IP ranges listed in https://ip-ranges.amazonaws.com/ip-ranges.json Where  "service" = "EC2".
(also ck-hub-preprod.crossknowledge.com for UAT)
```

### CK Flow (Nifi) IP addresses
```txt
Production : 3.125.172.227 ; 3.65.7.102 ; 3.64.247.80
```

## Email servers requirements

@crossknowledge.com domain must be whitelisted as a trusted sender.

### Supported email configuration scenario :

<table border="1" cellpadding="10" cellspacing="0">

<tbody><tr>
<td>All emails are sent by Amazon SES service from crossknowledge.com domain
</td>
<td>CKLS sends emails using a FROM address that belongs to crossknowledge.com domain only. (default and preferred solution)<br>
<p>The client's email address is kept in the REPLYTO field <br>
E.g&nbsp;: user john.doe@client.com sends an email to someone, the received email will have the following attributes <br>
</p>
<pre>FROM:noreply@crossknowledge.com
REPLYTO:john.doe@client.com
</pre>
</td></tr>
<tr>
<td>All emails are sent by Amazon SES service using a FROM address that belongs to the client's domain (or crossknowledge.com domain)
</td>
<td>
<p>This setup requires some extra IT configuration tasks for both CrossKnowledge and client's IT Teams&nbsp;: DKIM entries to be added in client's DNS zone&nbsp;: client.com. <br>
E.g mail can be sent from noreply@client.com or any other @client.com addresses. <br>
In case an email having a FROM attribute not belonging to either client.com or crossknowledge.com domain, the FROM attribute is automatically replaced by noreply@client.com or any other generic address chosen by the client during the setup phase.
Dedicated IPs can be used for whitelisting or security purposes.
</p>
</td></tr>
<tr>
<td>All emails are sent directly by the client's SMTP relay
</td>
<td>
<p>CKLS application is then authorized to directly pass emails flow to a remote client's relay using basic SMTP authentication method (login and password).<br>
CrossKnowledge will not provide any IP ranges (autoscalling CKLS servers may have various IPs changing regularly). SMTP session can be secured by a TLS connection. SMTP server (host and port), login and password to be provided by Client's Email team.<br>
 <b>WARNING:</b> Microsoft Office365 is not an viable option as the company <a href="[url](https://techcommunity.microsoft.com/t5/exchange-team-blog/basic-authentication-deprecation-in-exchange-online-may-2022/ba-p/3301866)">deprecated their basic authentication method on October 1st, 2022</a>
</p>
</td></tr></tbody></table>

Maximum message size (including attachments) is limited to 10 MB per message (after base64 encoding).

### Mail servers' IP addresses and whitelist

Current IP ranges used by AWS SES:
However these ranges may change, so to get an up to date list, please run the following command:
From a Linux or Mac OS system:
```txt
$ dig TXT amazonses.com +short| grep 'v=spf1'
```
From a Windows system
```txt
C:>nslookup -type=TXT amazonses.com | find "v=spf1"
```

### Hostnames of SMTP relays and custom MAIL FROM domains used for sending 	

```txt
email-smtp.us-east-1.amazonaws.com
sesmailna.crossknowledge.com
email-smtp.eu-west-1.amazonaws.com
sesmaileu.crossknowledge.com
```

## Sharepoint pre-requisites

### Sharepoint 2010
Microsoft Edge (latest version), Mozilla Firefox (latest version), Google Chrome (latest version)
### Sharepoint 2013
Microsoft Edge (latest version), Mozilla Firefox (latest version), Google Chrome (latest version)<br/>

{% include note.html content="This plugin is not supported on the latest version of Office 365 (SharePoint 2016)." %}

## URL of CKLS platform
### Supported formats

* https://customername.(eu,lms,na,sa,asia).crossknowledge.com

* https://customername.ckls.crossknowledge-china.com

* CrossKnowledge only supports HTTPS protocol with its own domains.

* Customers can manage their own URL (https://customername.customerdomain.com) using 301 or 302 HTTP redirects to the instance CrossKnowledge domain (https://customername.(eu,lms,na,sa,asia).crossknowledge.com or https://customername.ckls.crossknowledge-china.com)


### Sunset Assess&Test (Learnosity)

* We will sunset Assess&Test at the end of February 2025.
* The relateds URLs of Learnosity won't need to be whitelisted by customers and their partners starting from March 1 2025.
  

