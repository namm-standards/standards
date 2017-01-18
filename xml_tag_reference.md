## XML Tag Reference

### Coding Note

Below are tag-by-tag listings of each XML document in the NAMM B2B standard. Each tag is followed by a brief description and a flag indicating whether the tag is required in the particular document. Nested tags are indented to indicate the hierarchical structure of the documents.

Complex (parent) elements are shown here as separate start and end tags (e.g., <Location> ... </Location>), while simple (child) elements are shown as “empty” tags (e.g., <Name/>) for improved readability in this document. These tags would of course be coded in live documents with start tags, data, and end tags (e.g., <Name>MusicMax Corporation</Name>).

While most pertinent metadata in these documents is coded as nested tags (e.g., <Barcode> <ID>4959112079274</ID> <Type>GTIN-13</Type> </Barcode>), some metadata is coded instead as attribute/value pairs (e.g., <Price type="MSRP" Currency="USD">980.00</Price>). Attributes are shown here on separate lines below the tags to which they belong (as nested tags would be, except without enclosing <>s), and their descriptions begin with the notation "Attribute:".

Elements and attributes required by the XSD schemas are marked with an X in the **Req** column. If a child element or attribute is marked required but its parent element is not, it means that the parent is still optional but, if used, it must contain the required child elements or attributes.

***Important Note***: Most of the XML tags used in these files are mixed-case, as in <PartyIdType>; this coding technique is valid XML, and is used by design to improve human readability. However, XML code is case-sensitive, so users must be exceptionally careful to maintain proper tag case when creating and processing these files within their own editors, applications, and systems.

Party Document
Item Document
Functional Acknowledgement
Pricebook
Purchase Order
PO Status Request
PO Status / Det Ack
Advanced Shipping Notice
Invoice
Sell Through