---
description: A supplier invoice represents a billing document received from a supplier for goods or services, managed through the accounts payable process in Workday Financial Management.
layout: schema
name: Workday Supplier Invoice
properties_list:
- description: Workday ID (WID) uniquely identifying the supplier invoice
  name: id
  type: string
- description: Supplier-provided invoice number
  name: invoiceNumber
  type: string
- description: Supplier who issued the invoice
  name: supplier
  type: object
- description: Date on the invoice
  name: invoiceDate
  type: string
- description: Payment due date
  name: dueDate
  type: string
- description: Total invoice amount
  name: totalAmount
  type: number
- description: Total tax amount on the invoice
  name: taxAmount
  type: number
- description: Invoice currency
  name: currency
  type: object
- description: Current processing status of the invoice
  name: status
  type: string
- description: Company entity receiving the invoice
  name: company
  type: object
- description: Payment terms applied to the invoice (e.g., Net 30)
  name: paymentTerms
  type: string
- description: Individual invoice line items
  name: lines
  type: array
- description: Associated purchase order reference
  name: purchaseOrder
  type: object
- description: Worker who approved the invoice
  name: approvedBy
  type: object
- description: Timestamp when the invoice was created in Workday
  name: createdOn
  type: string
provider_name: Workday Financials
provider_slug: workday-financials
schema_file: json-schema/workday-financials-supplier-invoice-schema.json
slug: workday-financials-supplier-invoice
source_filename: workday-financials-supplier-invoice-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://community.workday.com/schemas/workday-financials/supplier-invoice.json\",\n  \"title\": \"Workday Supplier Invoice\",\n  \"description\": \"A supplier invoice represents a billing document received from a supplier for goods or services, managed through the accounts payable process in Workday Financial Management.\",\n  \"type\": \"object\",\n  \"required\": [\"invoiceNumber\", \"supplier\", \"invoiceDate\", \"totalAmount\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Workday ID (WID) uniquely identifying the supplier invoice\"\n    },\n    \"invoiceNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Supplier-provided invoice number\",\n      \"minLength\": 1\n    },\n    \"supplier\": {\n      \"$ref\": \"#/$defs/Reference\",\n      \"description\": \"Supplier who issued the invoice\"\n    },\n    \"invoiceDate\": {\n     \
  \ \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date on the invoice\"\n    },\n    \"dueDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Payment due date\"\n    },\n    \"totalAmount\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Total invoice amount\"\n    },\n    \"taxAmount\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Total tax amount on the invoice\"\n    },\n    \"currency\": {\n      \"$ref\": \"#/$defs/Reference\",\n      \"description\": \"Invoice currency\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Draft\", \"Approved\", \"Paid\", \"Canceled\"],\n      \"description\": \"Current processing status of the invoice\"\n    },\n    \"company\": {\n      \"$ref\": \"#/$defs/Reference\",\n      \"description\": \"Company entity receiving the invoice\"\n    },\n    \"paymentTerms\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Payment terms applied to the invoice (e.g., Net 30)\"\n    },\n    \"lines\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/InvoiceLine\"\n      },\n      \"description\": \"Individual invoice line items\"\n    },\n    \"purchaseOrder\": {\n      \"$ref\": \"#/$defs/Reference\",\n      \"description\": \"Associated purchase order reference\"\n    },\n    \"approvedBy\": {\n      \"$ref\": \"#/$defs/Reference\",\n      \"description\": \"Worker who approved the invoice\"\n    },\n    \"createdOn\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the invoice was created in Workday\"\n    }\n  },\n  \"$defs\": {\n    \"InvoiceLine\": {\n      \"type\": \"object\",\n      \"description\": \"An individual line item on a supplier invoice\",\n      \"properties\": {\n        \"lineNumber\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\"\
  : \"Line item number\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Description of the goods or services\"\n        },\n        \"quantity\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"description\": \"Quantity of items\"\n        },\n        \"unitCost\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"description\": \"Cost per unit\"\n        },\n        \"extendedAmount\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"description\": \"Total line amount\"\n        },\n        \"spendCategory\": {\n          \"type\": \"string\",\n          \"description\": \"Spend category for the line item\"\n        },\n        \"costCenter\": {\n          \"$ref\": \"#/$defs/Reference\",\n          \"description\": \"Cost center allocation\"\n        }\n      }\n    },\n    \"Reference\": {\n      \"type\": \"object\",\n      \"description\": \"A reference\
  \ to a related Workday resource\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Workday ID (WID) of the referenced resource\"\n        },\n        \"descriptor\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the referenced resource\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday-financials/refs/heads/main/json-schema/workday-financials-supplier-invoice-schema.json
tags:
- Accounting
- Cloud ERP
- Financial Management
- Procurement
title: Workday Supplier Invoice
---
