Invoice OCR Automation (AWS POC)

Problem Statement:
Manually validating invoices against Purchase Orders was time-consuming and error-prone in my procurement job.

Solution:
Created a POC on AWS using:
- S3 to store invoice PDFs
- Textract to extract text
- Lambda to process the data
- DynamoDB to store the data results.

How It Works:
1. Upload PDF invoice to S3
2. Lambda gets triggered
3. Textract extracts text (Invoice No, Amount, Date etc..)
4. Lambda compares with PO data
5. Result stored in DynamoDB

Architecture Diagram:
(see image below)

Skills Used:
AWS S3, Lambda, Textract, DynamoDB, IAM Roles

Business Impact:
Reduces invoice validation time from 2 hours to 10 minutes.
Improves accuracy.

