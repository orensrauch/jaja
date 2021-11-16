---
id: web-portal
title: Web Portal For SDE 7.3
layout: community
sectionid: community
permalink: community/web-portal.html

---


## Contents

- [Introduction](#introduction)
- - [About Safe-T SDE Server](#about-safe-t-sde-server)
- - [Prerequisites](#prerequisites)
- [Web Portal Features](#web-portal-features)
- - [Safe-T Outlook Plug-in](#safe-t-outlook-plug-in)
- [How To Log Into The Web Portal](#how-to-log-into-the-web-portal)
- [Web Portal Main Window](#web-portal-main-window)
- [Safe File Upload](#safe-file-upload)
- [Safe File Download](#safe-file-download)
- [Sending An Email Message](#sending-an-email-message)
- - [Email Composition Window](#email-composition-window)
- - [Email Send Options Window](#email-send-options-window)
- - [Email Security Levels](#email-security-levels)
- - [Send OTP Via SMS Or Email](#send-otp-via-sms-or-email)
- - [Attached Files Will Expire After](#attached-files-will-expire-after)
- - [Limit Amount Of Downloads](#limit-amount-of-downloads)
- - [Return Safe Receipt For Deliveries](#return-safe-receipt-for-deliveries)
- - [Safe Reply](#safe-reply)
- [Receiving A Secure Email](#receiving-a-secure-email)
- - [Receiving A High Security Email](#receiving-a-high-security-email)
- - [Receiving A Medium Security Email](#receiving-a-medium-security-email)
- - [Receiving A Low Security Email](#receiving-a-low-security-email)
- [Using The Online Viewer](#using-the-online-viewer)
- - [How To Preview A File](#how-to-preview-a-file)
- - [How To Email File Attachments That Cannot Be Downloaded](#how-to-email-file-attachments-that-cannot-be-downloaded)
- [Glossary](#glossary)


**Document Information**

This document is for informational purposes only. Safe-T Data makes no warranties, express or implied, in this document. Safe-T is a registered trademark of Safe-T Data A.R Ltd. in the United States and other countries. The names of other companies and products mentioned herein may be the trademarks of their respective owners.

The information contained in this document, or any addendum or revision thereof is proprietary of Safe-T Data A.R Ltd. and is subject to all relevant copyright, patent and other laws and treaties protecting intellectual property, as well as any specific agreement protecting Safe-T Data A.R Ltd. rights in the aforesaid information. Any use of this document or the information contained herein for any purposes other than those for which it was disclosed is strictly forbidden.

Safe-T Data A.R Ltd. reserves the right, without prior notice or liability, to make changes in equipment design or specifications. All specifications are subject to change without prior notice.

Safe-T Data A.R Ltd. assumes no responsibility for the use thereof nor for the rights of third parties, which may be affected in any way by the use thereof.

This document may contain flaws, omissions or typesetting errors; no warranty is granted nor liability assumed in relation thereto unless specifically undertaken in Safe-T Data A.R Ltd.’s sales contract or order confirmation. Information contained herein is periodically updated and changes will be incorporated into subsequent editions. If you have encountered an error please notify Safe-T Data A.R Ltd.


## Introduction
The Safe-T® Web Portal user's guide describes how end-users can securely store and share their important files. The web portal can be used in an organization that has deployed the Safe-T Secure Data Exchange server (SDE) version 7.4.

## About Safe-T SDE Server

SDE server enables organizations to securely exchange data of any type and size between people, applications, and businesses. It also furthers an organization's ability to enforce policies required to meet mandated security and privacy regulations.

SDE server can run a wide and flexible range of security tools to scan and encrypt files during the upload process before a user's files are stored in Safe Spaces. When a user downloads or shares files, SDE server automatically decrypts them.

## Prerequisites

Your IT administrator must do the following:

•	Create a user account for you in the Safe-T SDE server.

•	Provide a URL for accessing the web portal.

•	Provide you login credentials for authenticating at the web portal.

## Web Portal Features

Web portal users can do the following:

•	Store files in secure digital vaults called Safe Spaces.

•	Upload/download files securely to their Safe Spaces using a secure SSL channel. 

•	Access files created by other users if they have the correct permissions.

•	Share files by sending secure emails and file attachments.

•	Select a level of security (low, medium, high) applied to each sent email.

•	Send recipients emails that enable a 'Safe Reply' feature. This feature provides email recipients the capability to reply securely to the sender with a message and file attachments.

•	Display information about their sent emails.

 >Note: The web portal displays in a browser so there is no need for users to install additional software.

## Safe-T Outlook Plug-in

The Safe-T web portal is an alternative to using the Safe-T Outlook Plug-in. The web portal is designed for these use cases:

•	Your organization has decided not to deploy Microsoft Outlook.

•	You want to access Safe Spaces and files over the internet when you are outside your office.

## How To Log Into The Web Portal

Your IT administrator will provide you the following:

•	The Web portal URL 

•	Your user name + password.

**To log into the Safe-T web portal:**

1.	In a web browser, enter the URL of your organization's Safe-T web portal. 

The URL for the web portal should match this pattern: https://< SDE Server Host Name >/Safe-T/default.aspx.

A login window appears.

**Figure 1: Login Window With CAPTCHA Example**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/webportal/1.png?raw=true" alt="1" width="50%"/>

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/webportal/2.png?raw=true" alt="2" width="50%"/>

2.	Enter your user name and password.

3.	If your login screen displays a drop-down list for setting a language, leave the default value or select your preferred language.

4.	If a CAPTCHA appears, decipher it and enter the text you see. 

5.	Click Submit. 

## Web Portal Main Window

If you successfully authenticate at the web portal login screen, the main window appears.
 It displays all Safe Spaces and files you have permission to access.

**Figure 2: Web Portal Main Window**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/webportal/3.png?raw=true" alt="2" width="65%"/>

The following table describes the components of the main window.

**Table 1: Main Window Descriptions**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/webportal/4.png?raw=true" alt="2" width="65%"/>

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/webportal/5.png?raw=true" alt="2" width="65%"/>

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/webportal/6.png?raw=true" alt="2" width="65%"/>

**Figure 3: History Window Example**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/webportal/7.png?raw=true" alt="2" width="65%"/>

## Safe File Upload 

This section describes how to upload files from your computer to your Safe Space.

To upload files into your Safe Space:

1.	In the main window navigation panel, select the Safe Space or subfolder into which you want to upload files. 

2.	In the web portal main page, on the right side of the search box, there is an icon with an upward facing arrow. 

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/webportal/8.png?raw=true" alt="2" width="10%"/>

 
Click the icon. 

A browse window appears enabling you to upload files from your computer to the Safe Space or subfolder.

**Figure 4: File Upload Browse Window**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/webportal/9.png?raw=true" alt="2" width="65%"/>

3.	Select the files your want to upload to your Safe Space and click Open.

 >Note: According to your organization's security policies, files you upload will be scanned for malware, data loss, and then encrypted.


## Safe File Download 

This section describes how to download files from a Safe Space to your computer.

**To download files from a Safe Space to your computer:**

1.	In the web portal main page, select the checkbox on the left side of one, or more, files you want to download. 

2.	Do one of the following:

•	If you selected a single file, on the right side of the file's row, click the icon with the downward arrow. 

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/webportal/10.png?raw=true" alt="2" width="10%"/>
 
•	If you selected multiple files, in the upper right corner of the main window, click the icon with the downward arrow.
 
<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/webportal/11.png?raw=true" alt="2" width="65%"/> 

**A download window appears**

3.	Browse to the location on your computer where you want to download your files.

4.	Click Save. The Safe Space files you downloaded are copied to your computer 
  >Info: Files stored in your Safe Spaces in encrypted format are automatically decrypted when you download them.

## Sending An Email Message

This section describes how to use the web portal to send emails and file attachments.

## Email Composition Window

  >Info: When you send an email, you can either attach files stored in a single Safe Space, or you can select files from your computer, but you cannot do both.

 >Tip: To send file attachments from your Safe Space and from your computer in a single email: First upload the files you want from your computer to the Safe Space, then attach all the files from your Safe Space.

The following images show the email composition window that appears after you select either the airplane or envelope send email icon.

**Figure 5: Email Composition Window: File Attachments In Safe Space Or Stored In Your Computer**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/webportal/12.png?raw=true" alt="2" width="65%"/>

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/webportal/13.png?raw=true" alt="2" width="65%"/>

**The email composition window includes these components:**

•	Message tab: Enter the recipient's email address, compose a message, and add attachments.

•	Send Options tab: Configure an email security level, set the maximum number of file downloads allowed, enable 'Safe Reply', and more.

•	From: The sender is automatically configured to be the user who logged into the web portal.

•	To: Select or enter the recipient email address. If you type the email address, you must select the address when it appears in the drop-down list.

•	Subject: A concise summary telling the recipient the purpose of the email.

•	Message: Enter your email message.

•	Attachments: If you select files from your Safe Space before opening the email composition window, your attachments appear listed. 

•	Add Files: If you want to enter files stored in your computer, select the Add Files button. After you send these files as email attachments, they will be copied into your Safe Space.



## Email Send Options Window

This section describes how you can customize many important email send features.

Click the 'Send Options' tab to display the configuration options.


**Figure 6: Email Send Options**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/webportal/14.png?raw=true" alt="2" width="65%"/>

## Email Security Levels

The web portal provides three email security levels you can choose from: High, Medium, and Low. You can select a different security level each time you send an email.

  >Info: Your IT administrator may enforce a specific security level by disabling one or two of the security options. For example, your organization may disable the 'Low' security option.

  >Info: Recipients of medium and high security emails authenticate differently depending on whether they have SDE server user accounts. 

•	A recipient who is registered as a user in the SDE server authenticates with a company user name and password. 

•	A recipient who is not a part of your organization and is sent a medium or high security email will be sent an SMS, or a second email, containing an OTP verification code.

The following tables describe the three email security levels.


<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/webportal/15.png?raw=true" alt="2" width="80%"/>



## Send OTP Via SMS Or Email

If you send an email at a Medium or High security level, the recipient receives an email message that includes a download link: 'Secure Content'. 

When the recipient clicks 'Secure Content', members of your organization can log into the package download web page and access the secure content by entering their company user name and password.

External recipients, who do not have an SDE server user account, are required to enter an OTP verification code.

In the email composition Send Options tab, if you enable 'Send via SMS' the email recipient receives the OTP via SMS instead of by a separate email.

  >Info: In many organizations, an IT administrator will enforce a policy requiring all external email recipients to receive OTPs only via SMS. 

## Attached Files Will Expire After

You can set a duration in minutes, hours, days, or months after which your email recipients cannot use the Secure Content link to access the package you sent.

## Limit Amount Of Downloads

You can set a limit for the maximum number of times an email recipient can download file attachments from the package download web page.

## Return Safe Receipt For Deliveries

If you select this checkbox, when you send an email you receive information via a second email on the status of the email you sent.

**Figure 7: Example: Return Safe Receipt For Delivery**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/webportal/16.png?raw=true" alt="2" width="75%"/>

•	Package ID.

•	When the email was sent.

•	Attachment file names.

•	Attachment file sizes.

•	When the file attachments expire.

•	Maximum number of package downloads.

•	Number of times the package was downloaded.

•	Authentication method.

## Safe Reply

In Send Options, if you select the Safe Reply checkbox your email recipient can respond to you securely using a special type of email with file attachments. 

This feature is intended to enable individuals outside your organization, who do not have a Safe-T SDE server account, to send you secure email replies with file attachments.

  >Info: This feature must be enabled by your IT administrator in the SDE server.

**To send a Safe Reply**
1.	In the Send Options tab, select Safe Reply. 

2.	Send your email with attachments.

The recipient will receive an email with the following links.

**Figure 8: Safe Reply Link: Accept Invitation**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/webportal/17.png?raw=true" alt="2" width="65%"/>

3.	When the recipient clicks Accept Invitation a web page appears requiring authentication.

**Figure 9: Safe Reply Authentication**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/webportal/18.png?raw=true" alt="2" width="65%"/>

4.	The email recipient who wants to Safe Reply enters authentication credentials and clicks Submit.
 A window similar to the following appears.

**Figure 10: Safe Reply Email Composition Window**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/webportal/19.png?raw=true" alt="2" width="65%"/>

5.	The user replying must fill out the required fields and can optionally add files to reply to the original sender.

6.	Click Next. A confirmation window appears.

**Figure 11: Safe Reply Email Confirmation**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/webportal/20.png?raw=true" alt="2" width="65%"/>

7.	When you click Next the email reply and attachments are sent.

## Recipient Verification Code

When you send an email with file attachments using Medium or High security, recipients who are not registered as users in the SDE server receive an OTP either by SMS or a separate email.

The sender receives a message box displaying a copy of the recipient's verification code.

**Figure 12: Sender Receives A Copy Of The Verification Code**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/webportal/21.png?raw=true" alt="2" width="70%"/>
 

This feature enables the email sender to provide the OTP via mobile phone, or any other method, to the email recipient if for some reason the email recipient does not receive the OTP.

  >Info: This feature must be enabled by your IT administrator in the SDE server policies.

## Receiving A Secure Email

This section describes how to receive a secure email and attachments. 
The method is different depending on the level of security chosen by the email sender.

## Receiving A High Security Email

When a user sends a high security email, both the message and attachments are encrypted.
The recipient receives an email with an empty message area (some boilerplate text) and a link to download secure content. 

**Figure 13: Recipient Receives High Security Level Email**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/webportal/22.png?raw=true" alt="2" width="65%"/>

In a separate email, or in an SMS, the recipient is provided an OTP verification code. Registered users log in with their company login credentials. A typical verification code consists of 4 digits or letters (e.g. AQ91).

The recipient clicks the Secure Content link to display a Safe-T SDE Secure content download web page. The web page is for user authentication and looks similar to this: 


**Figure 14: Recipient Logs In By Entering OTP**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/webportal/23.png?raw=true" alt="2" width="65%"/>

The recipient enters the OTP verification code and clicks Submit.

If the verification code is correct, a web page displays the following information:

•	A decrypted message now is in clear text and viewable by the recipient. 

•	A link enabling the recipient to download the encrypted file attachment.

**Figure 15: Example Of Decrypted High Security Message**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/webportal/24.png?raw=true" alt="2" width="65%"/>

## Receiving A Medium Security Email

When a user sends an email using the Medium security level, the attachments are encrypted however the message is sent as clear text. 

In this example, a sender who submitted to the accounting department a travel expenses report did not think the message needed to be sent securely though the attached XLS file is encrypted.

**Figure 16: Recipient Receives Medium Security Email**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/webportal/25.png?raw=true" alt="2" width="65%"/>

The recipient, in this example the company's accounting department, receives an email with the sender’s message and a link for downloading Secure Content. 

In a separate email, or in an SMS, the recipient is provided with an OTP verification code. A typical verification code consists of 4 digits or letters (e.g. 32YH).

  >Info: The recipient views the sender’s message as plain text. However, the file attachments are stored securely in Safe Spaces.

The recipient clicks the Secure Content link to display a secure content download web page then enters the OTP and clicks Submit.

If the authentication is successful, a web page appears with a link that enables the recipient to download the encrypted file attachment.

## Receiving A Low Level Security Email

When a user sends an email using the Low security level, the file attachments are sent to email recipients with a link to download them securely from the Safe-T SDE server. 

**Figure 17: Recipient Receives a Low Security Email**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/webportal/26.png?raw=true" alt="2" width="65%"/>

Using Low security, recipients click Secure Content and can download the attachments without the need to provide authentication credentials.

  >Info: In this example, the sender did not consider the lunch invitation or the enclosed map to the Waffle House confidential enough to send using a higher level of security.

 >Note: Although the email recipient did not have to authenticate to access the attachment, the downloaded file was stored in an encrypted Safe Space and was downloaded by the recipient using a secure SSL channel.


## Using The Online Viewer

The Safe-T Online Viewer enables a Safe-T web portal user to do the following:

•	Preview a file stored in a Safe Space without downloading the file.

•	Send an email with file attachments that can be viewed by the email recipient online but cannot be downloaded.

## How To Preview A File

1.	Open the web portal.

**Figure 18: Files That Can Be Viewed Online**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/webportal/27.png?raw=true" alt="2" width="65%"/>


2.	Select the preview link of the file you want to preview. The contents of the file appear without downloading the file.


## How To Email File Attachments That Cannot Be Downloaded

1.	Open the web portal.

Select the file Send link. An email composition window opens.

**Figure 19: Select Allow Download/View Only Options**


<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/webportal/28.png?raw=true" alt="2" width="65%"/>

2.	Do either of the following:

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/webportal/29.png?raw=true" alt="2" width="65%"/>

**Example use case**: Susan wants to send James a pdf file that contains confidential information. 
Using the Safe-T web portal she selects the option ‘Allow View Only’ and sends James an email with the confidential pdf file attachment. 
James receives the email and can view the contents of the pdf online however he cannot download the pdf file.

## Glossary

This table describes some of the terminology used in this guide. 

**Table 5: Basic Terminology**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/webportal/30.png?raw=true" alt="2" width="65%"/>

