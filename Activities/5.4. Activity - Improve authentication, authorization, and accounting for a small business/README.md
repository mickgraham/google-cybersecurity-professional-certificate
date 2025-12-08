# Activity: Improve authentication, authorization, and accounting for a small business

*This activity is based on a fictional scenario.*

**References**

* **access-control-worksheet.docx:** Access control worksheet template
* **access-control-worksheet.docx-exemplar.docx:** Sample solution

## Scenario

You're the first cybersecurity professional hired by a growing business.

Recently, a deposit was made from the business to an unknown bank account. The finance manager says they didn't make a mistake. Fortunately, they were able to stop the payment. The owner has asked you to investigate what happened to prevent any future incidents.

To do this, you'll need to do some accounting on the incident to better understand what happened. First, you will review the access log of the incident. Next, you will take notes that can help you identify a possible threat actor. Then, you will spot issues with the access controls that were exploited by the user. Finally, you will recommend mitigations that can improve the business' access controls and reduce the likelihood that this incident reoccurs.

## Improve authentication, authorization, and accounting for a small business

| | Note(s) | Issue(s) | Recommendation(s) |
|-|---------|----------|-------------------|
| Authorisation/<br>Authentication | * The **Legal\Administrator** user made the payment<br>* The **Up2-NoGud** device was used | * The Legal account should not have access to make payments<br>* The device should not have been on the network | * Apply least privilege to remove access for the Legal department <br> * Improve device access controls |
