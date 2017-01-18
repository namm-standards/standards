## Transport Options

In the B2B scenario described above, the XML documents must be electronically transmitted between partners in order for data sharing to take place. Therefore, the transmission method used, called a transport protocol, must be understood and implemented by both parties to a transaction.

The set of protocols used for Internet communications is called the Internet Protocol Suite, commonly known as TCP/IP (Transmission Control Protocol/Internet Protocol). The two most popular transport protocols in use today are HTTP and FTP, discussed below.

### HTTP

HTTP (HyperText Transfer Protocol) can be used to upload (send) files from a local computer to a remote web server. This is the method used to download web pages from a server into a web browser for viewing, and to download auxiliary files from web pages to your local computer. In this scenario, a programmer must implement a system that runs a script or application so the sender can use it to upload a file. When the transfer is complete, the receiving system might then run another program to process the data (e.g., to input it into the company's accounting system). HTTP supports immediate in-session response, enabling the receiving party to validate the transmitted XML and respond by transmitting an XML document of its own (such as a Functional Acknowledgement) back to the sender. This type of transfer is typically used to send one file at a time (or multiple documents in an envelope).

### FTP
FTP (File Transfer Protocol) can also be used to upload files from a local computer to a remote location. In this scenario, the sender runs a specific kind of third-party application called an FTP client on their local computer to contact the recipient's server; the FTP client then lets the user select one or more files to transfer and sends them. FTP does not support immediate response; instead, transmitted files may be detected later by other software and managed in groups (batch processing). This type of transfer is typically used to send several files at a time.

### HTTP/FTP Comparison

**Transfer speed**: Both protocols have features that increase and decrease transmission speed. For example, while FTP does not take the time to "chunk" files as HTTP does, it uses two connections (one for commands and another for transfers) to accomplish its task. Conversely, while HTTP automatically compresses transmitted data, it adds metadata elements to the transmission stream. Ultimately, when transferring a small number of files that are not individually large (such as those in NAMM's B2B process), the speed difference is negligible.

**Security**: Neither standard HTTP nor FTP supports secure transmission, so each protocol has a secure version – HTTPS and SFTP – that can be used to provide secure file transfer between systems. Because FTP/SFTP, once connected, gives an authorized sender relatively broad access to the recipient's file system, where HTTP/HTTPS does not, additional software safeguards or strictly limited navigation permissions may be required. NAMM members are strongly encouraged to use the secure protocols (HTTPS/SFTP) in their B2B transactions to ensure the security and privacy of their communications.

**Popularity**: FTP is a much older system than HTTP, by a decade or more. Thus, historically speaking, FTP is more popular. However, because today virtually every page – and virtually every upload and download link – on the web is now served via HTTP, it is accurate to say that HTTP is by far the more popular protocol in terms of raw usage. Further, while there are many excellent and free FTP clients available (FireFTP, FileZilla, CoffeeCup Free FTP, WinSCP, etc.), HTTP/HTTPS is significantly easier to control and customize programmatically via browser scripting or programming languages, making it the most popular choice for developers of modern file transfer applications.

### Conclusion

XML files contain only "plain text" data, and thus are compatible with any transfer protocol. Which protocol you use is ultimately up to you and your business partners. You may in fact use both protocols to share data among partners, FTP for some and HTTP for others; or you might use FTP to send files and HTTP to receive them. The choice depends on what software you and your partner companies have available or are willing to develop.

## Resource Requirements

Implementing the NAMM B2B standard is not difficult and does not require specialized resources. Most likely, your company already has the basic facilities and resources required for implementation, such as:

* a web server that supports FTP or HTTP transport services
* an internet connection/hosting facility
* a domain name (or IP address)
* commercial or proprietary accounting software
* a software and/or web developer

You can get additional help with B2B planning and implementation at the NAMM web site (http://www.namm.org), through independent consultants, and from current B2B members. Certain third-party software packages such as point-of-sale products are popular with NAMM member organizations.

There are also many completely free XML tutorials, services, and utilities available online, such as the World Wide Web Consortium's (W3C) W3Schools training site (http://w3schools.com/xml/default.asp), XML editors like Microsoft's XML Notepad (http://www.microsoft.com/download/en/details.aspx?id=7973), and web-based validation tools such as DecisionSoft's online XML Schema Validator (http://tools.decisionsoft.com/schemaValidate/).

For more information or to ask specific questions, please email us at <dank@namm.org>