File transfer protocol
This is the standard internet protocol for file transfers between machines, addressing issues like differing coding systems, and file formats. FTP establishes two connections: a control connection for commands and responses, which remains open throughout the session, and a data connection for file transfer, which opens only when data is transferred. 

Simple mail transfer protocol (SMTP)
Email relies on SMTP for sending messages, requiring both client and server software to be constantly active to receive mail. Since emails can’t be received on a powered-off device, STMP is commonly paired with something called POP. with POP, emails are stored on a constantly running server, allowing the user to retrieve the email later via a client. A user agent interface typically assists in managing these tasks.
SMTP addresses consist of two parts:

- The local part (user mailbox name)
- The domain name (SMTP server’s computer)

Separated by an “@” sign. This format helps identify where each user’s emails and stored and retrieved. 

Ie, 
shauhonlau@gmail.com
shauhonlau@hotmail.com 
Same user mailbox names, different SMTP domains

Or, 

shauhonlau@gmail.com
sean.lau.25hotmail.25@gmail.com
Different user mailbox names, Same SMTP domains  (12 year old shau hon wasn’t very bright). 