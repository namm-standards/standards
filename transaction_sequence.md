## Transaction Sequence

A typical sequence of events between a product supplier and product buyer and the associated documents, in chronological order, might be as follows.

1. Both supplier and buyer complete and release mutually-available identification information in a **Party** document.
2. The supplier sends a catalog of available products to the buyer in an **Item** document.
3. The buyer acknowledges receipt of the Item document with a **Functional Acknowledgement** document.
4. The supplier sends a price list for available products to the buyer in a **PriceBook document** (optional).
5. The buyer acknowledges receipt of the PriceBook document with a Functional Acknowledgement document.
6. The buyer decides to purchase items from the catalog and sends a request for them to the supplier in a **Purchase Order document**.
7. The supplier acknowledges receipt of the Purchase Order with a **Functional Acknowledgement** document.
8. The buyer requests the status of their order with a **PO Status** Request document.
9. The seller provides the status of the order in a **PO Status Acknowledgement** document.
10. The supplier makes one or more product shipments to the buyer and sends detailed information for each shipment in an **Advanced Shipment Notification** document.
11. The buyer acknowledges receipt of the Advanced Shipment Notification with a **Functional Acknowledgement** document.
12. The supplier sends a request for payment to the buyer in an **Invoice** document.
13. The buyer acknowledges receipt of the Invoice with a **Functional Acknowledgement** document.
14. The supplier sends a report to the buyer indicating which products have been sold in a **SellThrough** document (optional).
15. The buyer acknowledges receipt of the SellThrough with a **Functional Acknowledgement document**.

Below is a diagram of this process, referencing the step/document numbers above.

![Image of Implementation Guide]
(https://namm-standards.github.io/standards/images/implementationguide_v2012-2.jpg)

*A typical B2B document transaction sequence*

