#Project Detail

This is a Mulesoft Project Used to Zip a folder which contains multiple file tested with size 500 mb + .
send the zip file through mail as an attachment.

#Configuration To be Done

Install New Software from:
http://anypoint-enterprise-security-update-site.s3.amazonaws.com/1.8.0

set your folder which you want to zip or the location of zip file to be sent from mail or the listener configuration in the following file.

src\main\resources\properties\sample-dev-file.yaml 

Email detail should be entered in the following file. I have used Gmail configuration.

src\main\resources\properties\secure\sample-dev-Email.properties

This properties file is password Encrypted . Password is present on the global property file ,with key value mule.key .

Algorithm used is BlowFish

password -> mule.key = sujal

Environment -> mule.env = dev

Email.userName -> Senders Gmail Username.

Email.password -> Password of sender's Gmail Id

Email.sendTo -> Recipient Gmail Username  

Enter the Email username and password and open the file using Mule Properties Editor and Encrypt at the same time using the Algorithm "BlowFish" and password as "sujal"

#point kept in mind

If the file is long , it will take time to run or send the mail, keep patience

Three Modules are used := secure Properties , Scripting , SMTP 

All the connectors configuration are present in Configuration.xml
