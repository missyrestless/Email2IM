# Email2IM

Email a message to a Second Life resident

## Table of Contents

- [INTRODUCTION](#introduction)
- [WHY BUY](#why-buy)
- [SETUP](#setup)
- [CONFIGURATION](#configuration)
- [USAGE](#usage)
- [FURTHER INFORMATION](#further-information)

## INTRODUCTION

The Email2IM object enables the owner to email a message to a Second Life resident. The object parses incoming email and relays the body of the message as an Instant Message to the Second Life resident whose name appears in the Subject line of the email. Owners of the Email2IM system are thus able to respond to forwarded IM's even when not online by simply sending email to the object's address with the name of the resident as the subject line.

In addition, the Email2IM object changes shape and texture, acting as an art object so as to be pleasing to the eye while in use.

## Why Buy

`Question`: Why should you buy these from me in Second Life or on the Second Life Marketplace rather than just download the git repository and deploy for free?

`Answer`: You are welcome to download and deploy for free. However, you may consider the following factors:

  - The products are extremely inexpensive
  - Sales support further development, better products, and new products
  - I probably know better than you how to package these for deployment in SL
  - You get some limited Support if you purchase from me
  - The time you spend downloading and deploying is worth a LOT more than the cost of buying

BUT, you might learn something by doing it all yourself so please feel free to dive in!

## SETUP

Simply rez the Email2IM object and position it where you would like the art display. Should you wish to modify the default values for length of interval between email checks, use of hover text, or restricting incoming email to a specific address then edit the configuration notecard "Email2IM_Config" in the object's contents. Configuration modification details are provided below.

## CONFIGURATION

The Email2IM script defaults can be modified by editing the Email2IM_Config notecard in the object's contents. To do so, right click the Email2IM object and select "Edit". In the edit window, click on the "Contents" tab. In the Contents tab, right click on the notecard "Email2IM_Config" and select "Open". You can now modify the following default values:

**`INTERVAL`**
  This value sets the time (in seconds) between checking for new email and changing the shape of the object. The default value is 120 seconds. The shape changes will be an integer multiple of this value.

**`MULTIPLE`**
  This value determines the interval at which shape changes occur. Values represent an integer multiple of the `INTERVAL` above. The default value is 1 meaning shape changes occur every time mail is checked. A value of 3 would mean shape changes occur every (3 * INTERVAL) seconds. A value of 0 means no shape or texture changes would occur.

**`HOVER_TEXT`**
  Set to TRUE or FALSE, this value determines whether or not the object will display it's status as hover text. Default value is TRUE.

**`ROTATE`**
  Set to FALSE if you do not wish the prim to rotate. Default TRUE.

**`SENDER`**
  If you wish to restrict the incoming email to only that sent from a particular email address then set SENDER to your email address. The default is to accept all incoming email and attempt to relay the message to the Subject. Should the Email2IM object's UUID be known to other parties then they would be able to flood the object with email. This parameter can be used to restrict email to only the owner or a trusted friend's email address.

**`SIMPLE`**
  Set to TRUE or FALSE. If you just want a small static box then set this to TRUE. If you want the prim to rotate and change textures/shape then leave it commented out. Setting this to TRUE also sets MULTIPLE above to 0 and SIZE below to small.

**`SIZE`**
  Some size defaults. This can be set to tiny, small, medium, large, XL, or XXL which will size the prim to 0.1, 0.5, 1.0, 2.0, 3.0, or 4.0 meters on a side.

While editing the Email2IM object you may also add or delete the textures in the object contents. These are used to periodically change the appearance of the various shapes. All textures in the object contents are automatically used. After completing any changes to the configuration notecard, save it and close the edit window. The object will reset with your changes in use.

## USAGE

Login to your Second Life dashboard at http://secondlife.com then click on "Account". Verify your email address and click on "Change Email Settings". Check the box for "I would like to receive offline IMs via Email". Click "Save Changes". You will now receive an email when offline and somebody IM's you.

When you rez the Email2IM object inworld and when you stop and restart it you will see the object's email address displayed in local chat. Copy and paste this email address into your addressbook or other document so you will have it available when offline. The object's email address will be of the form "UUID@lsl.secondlife.com". For example, if the objects UUID is 887047c4-d748-7888-3fd4-815f178ee03c then the email address to use to respond to IM's while offline would be 887047c4-d748-7888-3fd4-815f178ee03c@lsl.secondlife.com. Should you lose or forget your object's email address simply login, click the object to disable it, and click it again to re-enable it. The address will again be displayed in local chat.

When you receive a forwarded IM as an email message while offline you may wish to respond but do not wish to login to Second Life. This is where Email2IM comes in handy. You simply copy the name of the Second Life resident who sent you the IM and paste that into the Subject line of a new email. Address the email to the Email2IM object's email address that you determined in the previous paragraph. Write your reply as the body of the email message and send! For instance, to send an IM reply to Second Life resident Junior Allstar using the example Email2IM object UUID in the previous paragraph, you would send the following email message:

	To:  887047c4-d748-7888-3fd4-815f178ee03c@lsl.secondlife.com
	Subject: Junior Allstar

	Hi Junior! Got your IM but will not be available till Friday. See you then!
	Bob Dobbs

The Email2IM relay system uses the Second Life name to key service at http://w-hat.com/name2key. Should a name to key lookup fail for some reason, an IM will be sent to your Second Life account notifying you of the failure and name involved. Should you wish, you can locate this resident's key (at the top of their profile) and add it to the key database at the above url.

## FURTHER INFORMATION

The Email2IM product can be purchased on the Second Life Marketplace at http://tinyurl.com/4h6gvqk

This document is available in OpenOffice and PDF formats at https://www.scribd.com/document/904208538/Email2IM-Owner-Manual

Email missyrestless@gmail.com with any questions, comments, suggestions, etc.

View other Truth & Beauty Lab creations in the Second Life Marketplace at http://tinyurl.com/2bq6o3p
