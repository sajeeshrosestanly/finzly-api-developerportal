---
title: Wired Organization
---



## **Wire Origination**

Fedwire Funds service supports the following origination gateways for processing through BankOS 

` `- API – Finzly Connect APIs

- ` `Supports the initiation of
  - Customer or Corporate credit transfer 
  - Customer Transfer Plus 
  - Customer or Corporate Drawdown Request

` `- Web - Online Digital Treasury Portal (CashOS)

- Supports the initiation of domestic wire transfer
  - ` `This will be defined based on the Processing speed as Express (Configurable) and Fees to be applied.

\-  Branch - Teller Application (Wire Room) 

- Supports the initiation of Wire from branch using the teller application with an option as
  - Walk-in 
  - Phone-in

\-  Bulk uploads 

- Supports the initiation of wire with an option from Bulk File processing
  - ` `Fedwire message upload 
    - This will be based on the actual raw Fedwire message structure.
    - Multiple Fedwire message can be uploaded in a File

\-   Finzly CSV

- This is customed CSV formatted file for processing the Fedwire payments with required information as
  - Sender (Originator details) 
  - Sender A/c o Receiver (Beneficiary details) 
  - Receiver A/c 
  - Additional Notes
- Finzly CSV supports the following Business Function code
  - Customer or Corporate credit transfer 
  - Customer or Corporate Drawdown Request


### **Payment Status Updates**
  - __Payment Status Notification for every event on the wire life cycle will be notified. This will be applied for both outgoing and incoming payments.__
  - __Validation Failed - Fedwire Payment with the Exception status will be notified.__ 
  - __OFAC Review/Reject - Fedwire Payment with OFAC compliance Exception will be notified.__
  - __Memo Post Status - Fedwire Payment with memo post status failure will be notified.__
  - __### Processed - Notification back to the Customer on payment Processing.__

### **Drawdown Initiation**
- __Capability to initiate a Drawdown request for both Customer and as well as for the Bank for their treasury Funds/Fed Transfers.__
  - Drawdown initiation is possible for customer using the open Banking API and Bulk Files.
  - Every Drawdown request initiated will be received as a Separate drawdown payment linking the original payment. 
