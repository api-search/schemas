---
description: An accounts payable invoice in Oracle Fusion Cloud ERP representing a financial obligation to a supplier for goods or services received, including header information, line items, and payment details.
layout: schema
name: Oracle Fusion Cloud Invoice
properties_list:
- description: Unique system-generated identifier for the invoice
  name: InvoiceId
  type: integer
- description: Supplier-assigned invoice number
  name: InvoiceNumber
  type: string
- description: Total invoice amount in the invoice currency
  name: InvoiceAmount
  type: number
- description: ISO 4217 currency code for the invoice amount
  name: InvoiceCurrencyCode
  type: string
- description: Date of the invoice as provided by the supplier
  name: InvoiceDate
  type: string
- description: Classification of the invoice type
  name: InvoiceType
  type: string
- description: Name of the supplier who issued the invoice
  name: VendorName
  type: string
- description: Unique supplier number in the system
  name: VendorNumber
  type: string
- description: Supplier site from which the invoice originates
  name: VendorSiteCode
  type: string
- description: Business unit responsible for the invoice
  name: BusinessUnit
  type: string
- description: Free-text description of the invoice
  name: Description
  type: string
- description: Payment terms (e.g., Net 30, 2/10 Net 30)
  name: PaymentTerms
  type: string
- description: Date by which payment is due
  name: DueDate
  type: string
- description: Date used for accounting and period determination
  name: AccountingDate
  type: string
- description: Current status in the approval workflow
  name: ApprovalStatus
  type: string
- description: Validation status indicating whether the invoice passed validation checks
  name: ValidationStatus
  type: string
- description: Amount already paid against this invoice
  name: PaidAmount
  type: number
- description: Remaining unpaid amount
  name: AmountDue
  type: number
- description: Username of the person who created the invoice
  name: CreatedBy
  type: string
- description: Timestamp when the invoice record was created
  name: CreationDate
  type: string
- description: Timestamp when the invoice was last modified
  name: LastUpdateDate
  type: string
provider_name: Oracle Fusion Cloud Applications
provider_slug: oracle-fusion
schema_file: json-schema/oracle-fusion-invoice-schema.json
slug: oracle-fusion-invoice
source_filename: oracle-fusion-invoice-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.oracle.com/schemas/oracle-fusion/invoice.json\",\n  \"title\": \"Oracle Fusion Cloud Invoice\",\n  \"description\": \"An accounts payable invoice in Oracle Fusion Cloud ERP representing a financial obligation to a supplier for goods or services received, including header information, line items, and payment details.\",\n  \"type\": \"object\",\n  \"required\": [\"InvoiceNumber\", \"InvoiceAmount\", \"InvoiceCurrencyCode\", \"VendorName\", \"BusinessUnit\"],\n  \"properties\": {\n    \"InvoiceId\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique system-generated identifier for the invoice\"\n    },\n    \"InvoiceNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Supplier-assigned invoice number\",\n      \"minLength\": 1,\n      \"maxLength\": 50\n    },\n    \"InvoiceAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Total invoice amount\
  \ in the invoice currency\"\n    },\n    \"InvoiceCurrencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code for the invoice amount\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"InvoiceDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of the invoice as provided by the supplier\"\n    },\n    \"InvoiceType\": {\n      \"type\": \"string\",\n      \"enum\": [\"Standard\", \"Credit Memo\", \"Prepayment\", \"Mixed\"],\n      \"description\": \"Classification of the invoice type\"\n    },\n    \"VendorName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the supplier who issued the invoice\"\n    },\n    \"VendorNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Unique supplier number in the system\"\n    },\n    \"VendorSiteCode\": {\n      \"type\": \"string\",\n      \"description\": \"Supplier site from which the invoice originates\"\n    },\n    \"BusinessUnit\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Business unit responsible for the invoice\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Free-text description of the invoice\",\n      \"maxLength\": 240\n    },\n    \"PaymentTerms\": {\n      \"type\": \"string\",\n      \"description\": \"Payment terms (e.g., Net 30, 2/10 Net 30)\"\n    },\n    \"DueDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date by which payment is due\"\n    },\n    \"AccountingDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date used for accounting and period determination\"\n    },\n    \"ApprovalStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\"Initiated\", \"Required\", \"Not Required\", \"Approved\", \"Rejected\", \"Wfapproved\", \"Manually Approved\"],\n      \"description\": \"Current status in the approval workflow\"\n    },\n    \"ValidationStatus\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Validation status indicating whether the invoice passed validation checks\"\n    },\n    \"PaidAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Amount already paid against this invoice\",\n      \"minimum\": 0\n    },\n    \"AmountDue\": {\n      \"type\": \"number\",\n      \"description\": \"Remaining unpaid amount\"\n    },\n    \"CreatedBy\": {\n      \"type\": \"string\",\n      \"description\": \"Username of the person who created the invoice\"\n    },\n    \"CreationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the invoice record was created\"\n    },\n    \"LastUpdateDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the invoice was last modified\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-fusion/refs/heads/main/json-schema/oracle-fusion-invoice-schema.json
tags:
- Cloud
- CX
- Enterprise
- EPM
- ERP
- HCM
- Project Management
- REST API
- SaaS
- SCM
title: Oracle Fusion Cloud Invoice
---
