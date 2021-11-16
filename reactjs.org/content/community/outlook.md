---
id: outlook
title: Outlook Plugin User’s Guide
layout: community
sectionid: community
permalink: community/outlook.html
---

Microsoft® Outlook® Plug-in For SDE User’s Guide


## Contents

- [About This Guide](#about-this-guide)
- [Prerequisites](#prerequisites)
- [Terminology](#terminology)
- [Overview of the Safe-T SDE Outlook Plug-in Interface](#overview-of-the-safe-t-sde-outlook-plug-in-interface)
  - [Outlook Plug-in Interface Components](#outlook-plugin-interface-components)
- [Understanding Security Levels](#understanding-security-levels)
- [Sending a Secure Email](#sending-a-secure-email)
- [Receiving A Secure Email](#receiving-a-secure-email)
  - [Receiving A High Security Email](#receiving-a-high-security-email)
  - [Receiving A Normal Security Email](#receiving-a-normal-security-email)
  - [Receiving A Low Level Security Email](#receiving-a-low-level-security-email)
- [Transferring Large Size Files](#transferring-large-size-files)
- [Understanding Safe-Reply](#understanding-safe-reply)
- [Configuring Connection Settings](#configuring-connection-settings)
- [Configuring Global Send Options Parameters](#configuring-global-send-options-parameters)
  - [Safe-T Global Settings](#safe-t-global-settings)
- [Safe-t Global Send Options](#safe-t-global-send-options)
  - [Setting Package Delivery Parameters](#setting-package-delivery-parameters)
  - [Setting File Delivery Parameters](#setting-file-delivery-parameters)
  - [Setting File Safe Reply Parameters](#setting-file-safe-reply-parameters)
- [Safe-T New Email Send Options](#safe-t-new-email-send-options)
- [Using SmarTranfer](#using-smarTranfer)
  - [Accessing SmarTransfer From the New Email Window](#accessing-smartransfer-from-the-new-email-window)
  - - [Inserting an Attachment From the SmarTransfer Window](#inserting-an-attachment-from-the-smartransfer-window)
  - - [Other Tasks You Can Perform In The SmarTransfer Window](#other-tasks-you-can-perform-in-the-smartransfer-window)
- [Package Receipt](#package-receipt)
- [Sent Items Menu](#sent-items-menu)
  - [Package Properties](#package-properties)
  - [Viewing the Email Recipient’s Verification Code](#viewing-the-email-recipients-verification-code)

**Document Information**

This document is for informational purposes only. Safe-T Data makes no warranties, express or implied, in this document. Safe-T Data is a registered trademark of the Safe-T Data Corp. in the United States and/or other countries. The names of other companies and products mentioned herein may be the trademarks of their respective owners.

The information contained in this document, or any addendum or revision thereof is proprietary of Safe-T Data A.R., Ltd. and is subject to all relevant copyright, patent and other laws and treaties protecting intellectual property, as well as any specific agreement protecting Safe-T Data A.R., Ltd. rights in the aforesaid information. Any use of this document or the information contained herein for any purposes other than those for which it was disclosed is strictly forbidden. 

Safe-T Data A.R., Ltd. reserves the right, without prior notice or liability, to make changes in equipment design or specifications. All specifications are subject to change without prior notice. 
Safe-T Data A.R., Ltd. assumes no responsibility for the use thereof nor for the rights of third parties, which may be affected in any way by the use thereof. 

This document may contain flaws, omissions or typesetting errors; no warranty is granted nor liability assumed in relation thereto unless specifically undertaken in Safe-T Data A.R., Ltd.’s sales contract or order confirmation. Information contained herein is periodically updated and changes will be incorporated into subsequent editions. If you have encountered an error, please notify Safe-T Data A.R., Ltd. 

------------

## About This Guide

This user’s guide describes how to use the Microsoft® Outlook® Plug-in for Safe-T Secure Data Exchange server (SDE) version 7.1.0.

The Outlook Plug-in enables you to work with the familiar Outlook email client while taking advantage of many additional features such as:

* Enhanced security for emails and file/folder attachments

* The ability to send files and folders of any size

* The ability to manage data you store in Safe Spaces

This guide assumes you already are familiar with how to send and receive emails and other basic features of the Microsoft Outlook email client.

## Prerequisites

In order to use the plug-in, you need to obtain access to Microsoft Outlook with the Safe-T Outlook Plug-in application installed. You must also configure the connection details that enable the Outlook plug-in to communicate with the Safe-T SDE server.
 >Note: Your company’s system administrator will usually install and configure the Outlook Plug-in.

## Terminology

This table describes terms that are used in this guide. You should be familiar with them before continuing.

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/1.jpg?raw=true" alt="1" width="70%"/>

## Overview of the Safe-T SDE Outlook Plug-in Interface

This section provides a high-level overview describing how you can access the Secure Transport features within the Outlook Plug-in interface.

Starting in your Outlook email client, select the Home tab > New Email > Secure Transport tab. A new message window appears displaying the Outlook Plug-in icons. 

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/2.png?raw=true" alt="2" width="70%"/>

## Outlook Plug-in Interface Components

This table describes the main Outlook Plug-in components available to you in the Plug-in ribbon. Subsequent sections in this guide explain each of the features in greater detail.

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/3.jpg?raw=true" alt="3" width="70%"/>

 >Note: You can attach files and folders using either Insert File/Folder or SmarTransfer in each email you send but not both. To send file attachments from your local computer and from Safe Spaces you need to send separate emails.

## Understanding Security Levels

The Outlook Plug-in provides three security levels you can choose from: High, Normal, and Low. You select a security level each time you send an email.

 >Tip: Your system administrator may enforce using a particular security level, for example High, by disabling (greying out) a security option.

The following tables describe the available email security levels:

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/4.jpg?raw=true" alt="4" width="70%"/>

Select the High security level to encrypt both your email message and file/folder attachments. For example, if you send someone an email detailing your company’s business plans for the next quarter and include charts in an attached PPT presentation you should encrypt both the email message and attachment. 

  >Info: The High security level encrypts both the email message and file/folder attachments in an Outlook Safe Space on the Safe-T SDE server. When a recipient logs in to download them, they are decrypted and streamed over a secure protocol to the recipient.

**Normal**:
Similar to the High security level except the file/folder attachments are encrypted but the email message is not. Recipients are required to authenticate using an OTP verification code before accessing the file/folder attachments.
>Note: Registered recipients log in using their own login credentials instead of the OTP verification code.

The Normal security level encrypts your file/folder attachments. For example, if you send a business partner a PDF file containing an order form the email message itself might not require encryption though the file/folder attachments should be.

**Low**: 
The file/folder attachments are made available to your email recipients by sending them a link to download the files securely from the Safe-T SDE server. Using Low security, recipients do not have to authenticate.

## Sending a Secure Email 

This section describes the essential steps to send secure emails with attachments.

**To send a secure email:**

1.	New Email > Secure Transport tab > Secure Transport(On). The Outlook Plug-in toolbar interface appears. 

2.	Select the email security level you want: High, Normal, or Low.

3.	Fill out the To, Subject, and your message.

4.	Insert a file attachment using either Insert File/Folder or SmarTransfer.

 	The Insert File/Folder button provides the same functionality as the Outlook Message > Attach file paper clip icon in Outlook. Click the button and browse on your local computer for files you want to attach.
 	The SmarTransfer button enables you to attach files that are stored in your Safe Spaces. Click the button and browse in your Safe Spaces for files you want to attach as links.

 >Note: 1. If you right-click a file, the context menu includes a link: “Safe-T Secure Transport”. Click the link and the file you selected is loaded into the new email window as an attachment. You can insert file/folder attachments using either Insert/File Folder or SmarTransfer but in a given email you can use only one of the methods. 

2. To send file attachments from your local computer and from Safe Spaces, you need to send the file attachments in separate emails.

## Receiving A Secure Email
This section describes how to receive a secure email and attachments. The method is different depending on the level of security chosen by the email sender.

### Receiving A High Security Email
When a user sends a high security email, both the message and attachments are encrypted.

The recipient receives an email with an empty message area (some boilerplate text) and a link to download secure content. In a separate email, or in an SMS, the recipient is provided with an OTP verification code. Registered users log in with their own login credentials.

  >Info: The recipient cannot view the sender’s message in the email. The sender’s email message and file/folder attachments are stored securely on the Safe-T SDE server.

**Figure 5: Recipient Receives High Security Level Email**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/5.png?raw=true" alt="5" width="70%"/>

In a second email, or by SMS, the recipient gets an OTP verification code. A typical verification code consists of 4 digits (e.g. 8240).

The recipient now can click the Secure Content link to display a Safe-T SDE Secure content download web page. The web page is for user authentication and looks similar to this: 

**Figure 6: Recipient Logs In By Entering OTP**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/6.png?raw=true" alt="6" width="70%"/>

**The recipient enters a verification code and clicks Submit.**

If the verification code is correct, a web page displays the following information:

•	A decrypted message now viewable by the recipient. 

•	A link enabling the recipient to download the encrypted file attachment.

**Figure 7: Decrypted High Security Message**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/7.png?raw=true" alt="7" width="70%"/>

 >Tip: The file attachment is stored securely on the Safe-T SDE server. When the recipient authenticates using the verification code, the file can be downloaded. File or zipped folder attachments are always downloaded from the Safe-T SDE server using a secure communications protocol.

When the recipient downloads a file attachment, the sender receives an email report update noting that the email recipient downloaded a file attachment you sent. For more information, see the section describing the Package Receipt.

**Figure 8: Sender Receives a Delivery Receipt**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/8.png?raw=true" alt="8" width="70%"/>

### Receiving A Normal Security Email

When a user sends an email using the Normal security level, the attachments are encrypted however the message is not. 

In this example, a sender who submitted to the accounting department a travel expenses report did not think the message needed to be sent securely though the attached XLS file is encrypted.

**Figure 9: Recipient Receives Normal Security Email**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/9.png?raw=true" alt="9" width="70%"/>

The recipient, in this example the company accounting department, receives an email with the sender’s message visible and a link for downloading Secure Content. In a separate email, or in an SMS, the recipient is provided with an OTP verification code. A typical verification code consists of 4 digits (e.g. 9243).

  >Info: The recipient views the sender’s message as plain visible text. However, the file/folder attachments are stored securely on the Safe-T SDE server.

The recipient clicks the Secure Content link to display a secure content download web page. The web page is for user authentication and will look similar to this:

**Figure 10: Recipient Enters OTP Verification code**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/10.png?raw=true" alt="10" width="70%"/>

The recipient enters the verification code and clicks Submit.

If the verification code is correct, a web page appears with a link that enables the recipient to download the encrypted file attachment.

**Figure 11: Download Normal Security Attachments**
<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/11.png?raw=true" alt="11" width="70%"/>

 >Tip: The file attachment is stored securely on the Safe-T SDE server. When the recipient authenticates using the verification code the file can be downloaded. The file/folder attachments are always downloaded from the Safe-T SDE server using a secure communication protocol.

When the recipient downloads a file attachment, the sender receives an email update report noting the recipient downloaded a file attachment you sent.

**Figure 12: Sender Receives a Delivery Receipt**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/12.png?raw=true" alt="12" width="70%"/>

### Receiving A Low Level Security Email

When a user sends an email using the Low security level, the file/folder attachments are sent to email recipients with a link to download them securely from the Safe-T SDE server. Using Low security, recipients do not have to authenticate.

**Figure 13: Recipient Receives a Low Security Email**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/13.png?raw=true" alt="13" width="70%"/>

In this example, the sender did not consider the lunch invitation or the enclosed map to the Waffle House confidential enough to send using a higher level of security.

However, email attachments sent using the Low security level are downloaded from the Safe-T SDE server using a secure HTTPS network link.

## Transferring Large Size Files

An advantage of using Safe-T SDE, in addition to enabling secure data storage and transfer, is the capability to send files of any size, for instance 5GB. If upload or download times become lengthy you can send large files from a dedicated client computer or send the files overnight. 

 >Tip: If you do not want to encrypt large files, you can send them using the Low security level.
  >Info: Microsoft Outlook blocks sending or receiving attachments that exceed 20 MB and often company system administrators set a limit of 10 MB. Using Safe-T SDE, you can easily send them.

## Understanding Safe-Reply

The Safe-Reply invitation allows your email recipient to respond securely to you in an email with secure attachments.

 >Tip: Individuals outside your organization do not have a Safe-T SDE account or any additional software installed. They can send you safe email replies securely that include large file/folder attachments.

**Figure 14: Send a Safe-Reply Invitation**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/14.png?raw=true" alt="14" width="70%"/>

To send a Safe-Reply invitation: In a new email > Secure Transport On > click the Safe-Reply checkbox > set the security level to either Normal or High.

The email recipient receives a verification code and a separate email that looks similar to this:

**Figure 15: Recipient Receives a Delivery Receipt**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/15.png?raw=true" alt="15" width="70%"/>

**Secure Content link**: Access the sender’s message (if the security level=High) and attachments. You need to enter your verification code in an authentication web page.

**Accept Invitation link**: Access a web page that enables you to reply one time securely to the sender with a message and attachments. You need to enter your verification code in an authentication web page.

**Figure 16: Recipient Can Send a Safe Reply** 

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/16.png?raw=true" alt="16" width="70%"/>

The recipient writes a message > adds file attachments > clicks Next.

A confirm details window appears. Click Next.

**Figure 17: Recipient Can Add File Attachments To The Safe Reply**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/17.png?raw=true" alt="17" width="70%"/>

The Safe-Reply is sent and a message appears: “Action completed successfully”.

The original sender receives an email with a Secure Content link. Clicking the link opens a Safe-T web download page into which the sender enters a verification code or is allowed to log in as a registered user. 

## Configuring Connection Settings


This section describes how to configure the connection details that enable the Outlook plug-in to communicate with the Safe-T SDE server.

 Note: Your company’s system administrator will usually install and configure the Outlook Plug-in.

**To open the connection settings window**

1.	In the Outlook client ribbon, click the Add-ins tab.

2.	Click the Safe-T button, then click Settings. A Settings window appears.

3.	Click the Connection tab if it is not already selected.

**Figure 18: Global Settings Connection Tab**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/18.png?raw=true" alt="18" width="70%"/>

**Enter values for these fields. Note that in general the connection details to the Safe-T SDE server are configured by your system administrator.**

•	**User name**: The Safe-T SDE server account user name.

•	**Password**: The Safe-T SDE server account password.

•	**RemoteUFID**: Identifier used to connect the Outlook Plug-in with a specific Safe Space in the Safe-T SDE server.

•	**Server Name or IP address**: Safe-T SDE server network address.

•	**Test Settings**: Click to verify you have a connection to the Safe-T SDE server. If you are connected a message appears: “Success. You have a valid connection”.

If you change any connection details, **click OK**.

## Configuring Global Send Options Parameters

Global features refer to parameters you can set as default values for all emails. They are applied whenever you send an email. However, these are exceptions:

•	Your system administrator can enforce all configuration parameters. When this occurs, the option you see is disabled (i.e. greyed out).

•	You can override global Send Option settings on an individual basis when you open a new email window. 


 >Note: This section describes only the most important configuration parameters.


## Safe-T Global Settings


You can automate when to send emails using the Plug-in Secure Transfer feature by setting a rule on how Safe-T SDE handles file attachments. 

When you send an email as an ordinary Outlook user without setting Secure Transport On, if your email and attachments meet the condition you set with this feature, Secure Transport will be automatically set to On.

**To set a file attachments rule:**

1.	In the Outlook Plug-in client, click Add-ins > Safe-T > Settings > Settings tab.


**Figure 19: Global Settings Tab**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/19.png?raw=true" alt="19" width="70%"/>

2.	**In Use Safe-T to send, select one of these options:**

•	All attachments: If your Outlook email contains a file attachment, Secure Transport will be turned on.

•	Attachments larger than: If your Outlook email contains a file attachment that is larger in size than a number you set (e.g. 15 MB), Secure Transport will be turned on.

  >Info:Microsoft Outlook blocks sending or receiving attachments that exceed 20 MB and often company system administrators set a limit of 10 MB. For more information, see Transferring Large Size Files.

•	Attachments on demand: Your Outlook email will be sent with Secure Transport Off, unless you click the Secure Transport tab and Secure Transport On.

•	All messages: Your Outlook email will be sent with Secure Transport whether you are sending a message with or without any file attachments.

•	Ask me before sending: If you select this option, when you click Send a prompt will display asking you if you want to send the email and attachments using either High, Normal, or Low security.

3.	When you are done making changes, click OK.

## Safe-T Global Send Options

Global Send Options refer to parameters you can set as default values for all emails. They are applied whenever you send an email. However, these are exceptions:
•	Your system administrator can enforce all configuration parameters. When this occurs, the option you see is disabled (i.e. greyed out).

•	You can override global Send Option settings on an individual basis when you open a new email window. 

 >Note: This section describes only the most important configuration parameters.

## Setting Package Delivery Parameters

**To Configure Send Options (Package Delivery Settings tab):**
In the Outlook Plug-in client, click Add-ins > Safe-T > Send Options > Package Delivery Settings tab.

**Figure 20: Global Send Options Package Delivery Tab**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/20.png?raw=true" alt="20" width="70%"/>

You can optionally configure these parameters:

•	**Package will expire after**: Set the duration in days after which your recipients cannot access your package using the Secure Content link in the email you send.

•	**Secure Deliver with OTP (One-Time Password)**: If you select the checkbox, your recipients will need to authenticate using a verification code that is sent to them either in a separate email, or by SMS. Note: Registered recipients log in using their own login credentials.

•	**Via Cell-Phone (SMS)**: If you select the checkbox, your recipients will receive an OTP verification code via SMS. By default, recipients are sent a verification code in a separate email.

•	**Cell-Phone auto-suggest**: When you send an email a prompt appears: “Enter recipient’s mobile number”. The prompt includes a link enabling you to browse the Microsoft Exchange Address Book for the recipient’s mobile phone number.

•	**Encrypt Message**: If you select the checkbox, the security level is set to High.

•	**Attachment Type**: Select how email recipients access attachments sent to them:

o	**Secure HTML**: Enclosed in the email there’s an HTML file. If you click, it a link appears “Click here to proceed...” that displays the web download page.

o	**Secure URL Link**: Embedded on top of the E-Mail Message Body (default):Displays the web download page.

o	**Secure Document**: Normal attachment: Displays the web download page.

•	**Limit amount of downloads per package:** Sets the limit on the number of times an email recipient can download file attachments from the secure content download web page.

•	**Package name**: Set the display text of the link email recipients can click on to download secure messages and file attachments. By default the link is: Secure Content.

When you are done making changes, click OK.

## Setting File Delivery Parameters

**To Configure Send Options (File Delivery Settings tab):**

In the Outlook Plug-in client, click Add-ins > Safe-T > Send Options > File Delivery Settings tab.

**Figure 21: Global Send Options File Delivery Tab**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/21.png?raw=true" alt="21" width="70%"/>

You can optionally configure these parameters:

•	**File Protection password**: If you enter a password, the file attachments you send will be encrypted. Your recipient needs to know the password you set in order to decrypt the files attachments you send.

 >Tip: If you send file attachments with High or Normal security, your email recipient must enter an OTP verification code and after file download must enter a separate password you optionally set using the file protection password feature.

•	**Encrypt file using AES**: If you select the checkbox, along with setting a file protection password, your files are encrypted with a strong encryption algorithm.

•	**Split files into smaller parts using zip compression:** If you send a large file attachment greater than the split size in MB, your file attachment is split into smaller zip files. By default, files are split if they are larger than 700MB.


## Setting File Safe Reply Parameters

**To Configure Send Options (Safe Reply tab):**

In the Outlook Plug-in client, click Add-ins > Safe-T > Send Options > Safe Reply tab.

**Figure 22: Global Send Options Safe Reply Tab**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/22.png?raw=true" alt="22" width="70%"/>

You can optionally configure these global send parameters:

•	**Invite recipients to a Safe Reply**: If you select the checkbox, your email recipient can respond securely to you in an email with secure attachments.

•	**Invitation will expire after**: Set a duration in days after which the recipient cannot send you a Safe Reply.

•	**Return Safe Receipt for Delivery**: If you select the checkbox, when the email recipient downloads a sent package from the Secure Content download web page, you will receive an email receipt with package details (e.g. ID, Date, Expiry Date, Max Downloads: # Package Read: Auth Method).

•	**Distribution Job**: Enables you to set the email sender’s name and email address to an arbitrary value. For example, you may want to send a bulk mailing using a company name instead of your own personal email name and address.

## Safe-T New Email Send Options

New Email Send Options refer to parameters you can set when you open a new email window. The settings apply only to the new email you are sending.

•	You can override the global Send Option settings on an individual basis for the new email. 

•	Your system administrator can enforce all configuration parameters. When this occurs, the option you see is disabled (i.e. greyed out).

 >Note: The Global and New Email Send Option parameters are the same. The difference is the global settings are the default settings, and the changes you make in the new Email Send Options dialog box override the global default values only for the individual new email you are sending.

For example, if you set a Global Send Option to limit the number of downloads for a secure package to 5 times, you can change that setting for an individual email to a value of 3 downloads.

**To open the new email Send Options window, do the following:**

Outlook > Home > New Email > Secure Transport > Send Options.

**Figure 23: New Email Send Options**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/23.png?raw=true" alt="23" width="70%"/>

## Using SmarTransfer 

**SmarTransfer** enables you to view, manage, and send files that are stored in your Safe Spaces. 

A Safe Space is a folder hosted on the Safe-T SDE server. You can upload/download files from a Safe Space, and you can insert files from a Safe Space into an email as an attachment. For more information, see Basic Terminology.

**You can access SmarTransfer in the Outlook Plug-in two ways:**

•	Outlook New Email Window.

•	Outlook client navigation pane.

## Accessing SmarTransfer From the New Email Window

To access the SmarTransfer window using the SmarTransfer button open a new email > Secure Transport tab > click the SmarTransfer button.

**Figure 24: New Email Send Options**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/24.png?raw=true" alt="24" width="70%"/>

The SmarTransfer window appears:

**Figure 25: SmarTransfer Safe Space Folders**


<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/25.png?raw=true" alt="25" width="70%"/>

>Tip: If you do not see the Safe Space folders, click the Home button. 

## Inserting an Attachment From the SmarTransfer Window

The files in Safe-T SDE are not stored in your local computer. They are in the Safe-T SDE server until you access them. 
  >Note: You can attach files using either Insert File/Folder or SmarTransfer in each email you send but not both. To send file attachments from your local computer and from Safe-T SDE you need to send separate emails.

**To insert a file from SmarTransfer as an email attachment**

1.	Double-click a Safe Space that contains a file you want to insert as an email attachment. 




**Figure 26: SmarTransfer Safe Space Files**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/26.png?raw=true" alt="26" width="70%"/>

2.	Select the file you want to attach and click Insert. A window similar to this appears:

**Figure 27: SmarTransfer File Attachment**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/27.png?raw=true" alt="27" width="70%"/>

>Info:  When you insert a file attachment from SmarTransfer, in your email attachments window you will see a link to the file in your Safe Space, not the actual file.

## Other Tasks You Can Perform In The SmarTransfer Window

SmarTransfer hosts Space Spaces that are folders and files managed by the Safe-T SDE server. In addition to inserting file attachments into an email you can do the following:

**Table 6: The SmarTransfer Ribbon Interface.**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/28.png?raw=true" alt="28" width="70%"/>


## Package Receipt

When you send a secure email, you have the ability to gain a lot of information about it. One source of details is in the package delivery receipt. After the recipient logs into the secure access portal and downloads attachments, you are sent a package delivery receipt.

For example:

**Figure 29: Package Delivery Receipt**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/29.png?raw=true" alt="29" width="70%"/>

**The delivery receipt provides these details:**

•	Package ID

•	Subject of the Email

•	Date sent

•	Date access to download the file attachments expires

•	Maximum number of times the attachments can be downloaded

•	Number of times the package was accessed

•	Authentication method

## Sent Items Menu

You can access another source of details about the emails and attachments you send by accessing the Sent Items [Safe-T SDE] link on the Outlook client navigation pane.

**Figure 30: Sent Items Link**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/30.png?raw=true" alt="30" width="70%"/>

Click Sent Items [Safe-T SDE] and a Package Details window appears.

**Figure 31: Package Details**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/31.png?raw=true" alt="31" width="70%"/>



**The Package Details window displays these details:**

•	Name of the sender and recipient.

•	Number of recipients to which the email was sent.

•	Date and time the email was sent.

•	Size of the file attachments in KB.

•	The IP address of the email sender.

•	Package Settings.

•	View OTP.

## Package Properties

In Package Properties you can add, replace, and delete file attachments. 
You can perform these modifications even after the file attachments have been accessed by the email recipient.

Click the Package Settings link then click Package Update to open the Package Properties window.

**Figure 32: Package Properties**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/32.png?raw=true" alt="32" width="70%"/>

**To add file attachments to the package:**

1.	Click Safe Upload.

2.	Browse to a file or files you want to add.

3.	Select the files and click Open.

The files are added to the email package. 

 <Note: After you add new files to the email package, if the email recipient clicks the Secure Content link and authenticates again using the verification code, the file attachments for the package will display the new files you added.

**To delete file attachments from the package:**

1.	Click the file or files you want to delete.

2.	Click Delete.

The files are deleted from the email package. 

To download file attachments from the package:

1.	Click the file or files you want to download.

2.	Browse to a location on your local computer.

3.	Click Save. 

The files are saved on your local computer. 

To share file attachments from the package:

1.	Click the file or files you want to share.

2.	Click Safe Share.

A new email window opens with the file or files you selected attached to the email as an attachment.

## Viewing the Email Recipient’s Verification Code

Occasionally, an email recipient may have trouble using the verification code sent to them to authenticate at the download package web page.

  >Info: If enabled by your system administrator, in the Package Details window there will be a View OTP link:

1.	Click the View OTP link and a message box appears displaying the recipient’s verification code.

**Figure 33: View Recipient’s OTP**

<img src="https://github.com/orensrauch/The_Software_Testing_Router/blob/main/outlook/33.png?raw=true" alt="33" width="70%"/>

2.	Click OK to close the window.


