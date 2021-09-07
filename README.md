# Day-5
30 Days of Codding 





Sending Attachments as an E-mail

To send an e-mail with mixed content requires to set Content-type header to multipart/mixed. Then, text and attachment sections can be specified within boundaries.

A boundary is started with two hyphens followed by a unique number, which cannot appear in the message part of the e-mail. A final boundary denoting the e-mail's final section must also end with two hyphens.

Attached files should be encoded with the pack("m") function to have base64 encoding before transmission.


Following is the code, which sends a file /tmp/test.txt as an attachment. 
