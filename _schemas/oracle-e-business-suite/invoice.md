---
description: Schema representing an Accounts Payable invoice in Oracle E-Business Suite. Maps to AP_INVOICES_ALL and AP_INVOICE_LINES_ALL tables. Covers standard invoices, credit memos, debit memos, and prepayments.
layout: schema
name: Oracle EBS Invoice
properties_list:
- description: Unique identifier for the invoice (AP_INVOICES_ALL.INVOICE_ID)
  name: invoiceId
  type: integer
- description: Supplier invoice number (AP_INVOICES_ALL.INVOICE_NUM)
  name: invoiceNum
  type: string
- description: Invoice date
  name: invoiceDate
  type: string
- description: Date the invoice was received
  name: invoiceReceivedDate
  type:
  - string
  - 'null'
- description: Invoice type lookup code
  name: invoiceType
  type: string
- description: Supplier/vendor identifier (AP_SUPPLIERS.VENDOR_ID)
  name: vendorId
  type: integer
- description: Supplier/vendor name
  name: vendorName
  type: string
- description: Vendor number
  name: vendorNum
  type: string
- description: Vendor site identifier (AP_SUPPLIER_SITES_ALL.VENDOR_SITE_ID)
  name: vendorSiteId
  type: integer
- description: Vendor site code
  name: vendorSiteCode
  type: string
- description: Total invoice amount in invoice currency
  name: invoiceAmount
  type: number
- description: Invoice currency code (ISO 4217)
  name: invoiceCurrencyCode
  type: string
- description: Payment currency code (ISO 4217)
  name: paymentCurrencyCode
  type: string
- description: Currency exchange rate
  name: exchangeRate
  type:
  - number
  - 'null'
- description: Exchange rate type (Corporate, Spot, User)
  name: exchangeRateType
  type:
  - string
  - 'null'
- description: Exchange rate date
  name: exchangeDate
  type:
  - string
  - 'null'
- description: Invoice amount in functional/base currency
  name: baseAmount
  type:
  - number
  - 'null'
- description: Payment terms identifier (AP_TERMS.TERM_ID)
  name: termsId
  type: integer
- description: Payment terms name
  name: termsName
  type: string
- description: Payment terms date
  name: termsDate
  type:
  - string
  - 'null'
- description: Invoice description
  name: description
  type:
  - string
  - 'null'
- description: Invoice source (Manual, EDI, ERS, etc.)
  name: source
  type: string
- description: 'Payment status: Y=Fully Paid, N=Not Paid, P=Partially Paid'
  name: paymentStatusFlag
  type: string
- description: Payment method lookup code
  name: paymentMethodCode
  type:
  - string
  - 'null'
- description: Approval status
  name: approvalStatus
  type: string
- description: Workflow approval status
  name: wfapprovalStatus
  type:
  - string
  - 'null'
- description: Total amount paid against this invoice
  name: amountPaid
  type: number
- description: Total discount amount taken
  name: discountAmountTaken
  type:
  - number
  - 'null'
- description: Amount applicable to discount
  name: amountApplicableToDiscount
  type:
  - number
  - 'null'
- description: Total tax amount
  name: taxAmount
  type:
  - number
  - 'null'
- description: Matched purchase order header ID
  name: poHeaderId
  type:
  - integer
  - 'null'
- description: Date goods were received
  name: goodsReceivedDate
  type:
  - string
  - 'null'
- description: General Ledger accounting date
  name: glDate
  type: string
- description: Pay group
  name: payGroupLookupCode
  type:
  - string
  - 'null'
- description: Date the invoice was cancelled
  name: cancelledDate
  type:
  - string
  - 'null'
- description: Cancelled amount
  name: cancelledAmount
  type:
  - number
  - 'null'
- description: Invoice lines
  name: lines
  type: array
- description: Payment records associated with this invoice
  name: payments
  type: array
- description: Active holds on this invoice
  name: holds
  type: array
- description: Operating unit identifier
  name: orgId
  type: integer
- description: User who created the record
  name: createdBy
  type: integer
- description: Record creation date
  name: creationDate
  type: string
- description: User who last updated the record
  name: lastUpdatedBy
  type: integer
- description: Record last update date
  name: lastUpdateDate
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/invoice.json
slug: invoice
source_filename: invoice.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.oracle.com/ebs/invoice.json\",\n  \"title\": \"Oracle EBS Invoice\",\n  \"description\": \"Schema representing an Accounts Payable invoice in Oracle E-Business Suite. Maps to AP_INVOICES_ALL and AP_INVOICE_LINES_ALL tables. Covers standard invoices, credit memos, debit memos, and prepayments.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"invoiceId\",\n    \"invoiceNum\",\n    \"vendorId\",\n    \"invoiceAmount\",\n    \"invoiceCurrencyCode\"\n  ],\n  \"properties\": {\n    \"invoiceId\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the invoice (AP_INVOICES_ALL.INVOICE_ID)\"\n    },\n    \"invoiceNum\": {\n      \"type\": \"string\",\n      \"description\": \"Supplier invoice number (AP_INVOICES_ALL.INVOICE_NUM)\",\n      \"maxLength\": 50\n    },\n    \"invoiceDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"\
  description\": \"Invoice date\"\n    },\n    \"invoiceReceivedDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Date the invoice was received\"\n    },\n    \"invoiceType\": {\n      \"type\": \"string\",\n      \"description\": \"Invoice type lookup code\",\n      \"enum\": [\n        \"STANDARD\",\n        \"CREDIT\",\n        \"DEBIT\",\n        \"PREPAYMENT\",\n        \"MIXED\",\n        \"EXPENSE REPORT\",\n        \"RETAINAGE RELEASE\"\n      ]\n    },\n    \"vendorId\": {\n      \"type\": \"integer\",\n      \"description\": \"Supplier/vendor identifier (AP_SUPPLIERS.VENDOR_ID)\"\n    },\n    \"vendorName\": {\n      \"type\": \"string\",\n      \"description\": \"Supplier/vendor name\",\n      \"maxLength\": 240\n    },\n    \"vendorNum\": {\n      \"type\": \"string\",\n      \"description\": \"Vendor number\"\n    },\n    \"vendorSiteId\": {\n      \"type\": \"integer\",\n      \"description\": \"Vendor site identifier\
  \ (AP_SUPPLIER_SITES_ALL.VENDOR_SITE_ID)\"\n    },\n    \"vendorSiteCode\": {\n      \"type\": \"string\",\n      \"description\": \"Vendor site code\"\n    },\n    \"invoiceAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Total invoice amount in invoice currency\"\n    },\n    \"invoiceCurrencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"Invoice currency code (ISO 4217)\",\n      \"pattern\": \"^[A-Z]{3}$\",\n      \"examples\": [\n        \"USD\",\n        \"EUR\",\n        \"GBP\"\n      ]\n    },\n    \"paymentCurrencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"Payment currency code (ISO 4217)\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"exchangeRate\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Currency exchange rate\"\n    },\n    \"exchangeRateType\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Exchange rate type (Corporate, Spot, User)\"\n    },\n    \"exchangeDate\"\
  : {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Exchange rate date\"\n    },\n    \"baseAmount\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Invoice amount in functional/base currency\"\n    },\n    \"termsId\": {\n      \"type\": \"integer\",\n      \"description\": \"Payment terms identifier (AP_TERMS.TERM_ID)\"\n    },\n    \"termsName\": {\n      \"type\": \"string\",\n      \"description\": \"Payment terms name\"\n    },\n    \"termsDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Payment terms date\"\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Invoice description\",\n      \"maxLength\": 240\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Invoice source (Manual, EDI, ERS, etc.)\",\n      \"maxLength\": 80\n    },\n    \"paymentStatusFlag\": {\n      \"type\":\
  \ \"string\",\n      \"description\": \"Payment status: Y=Fully Paid, N=Not Paid, P=Partially Paid\",\n      \"enum\": [\n        \"Y\",\n        \"N\",\n        \"P\"\n      ]\n    },\n    \"paymentMethodCode\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Payment method lookup code\"\n    },\n    \"approvalStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Approval status\",\n      \"enum\": [\n        \"APPROVED\",\n        \"NEEDS_REAPPROVAL\",\n        \"NEVER_APPROVED\",\n        \"CANCELLED\",\n        \"WFAPPROVED\",\n        \"MANUALLY APPROVED\"\n      ]\n    },\n    \"wfapprovalStatus\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Workflow approval status\",\n      \"enum\": [\n        \"REQUIRED\",\n        \"NOT REQUIRED\",\n        \"INITIATED\",\n        \"WFAPPROVED\",\n        \"REJECTED\",\n        \"MANUALLY APPROVED\",\n        null\n      ]\n    },\n    \"amountPaid\": {\n      \"type\": \"number\",\n\
  \      \"description\": \"Total amount paid against this invoice\",\n      \"minimum\": 0\n    },\n    \"discountAmountTaken\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Total discount amount taken\"\n    },\n    \"amountApplicableToDiscount\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Amount applicable to discount\"\n    },\n    \"taxAmount\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Total tax amount\"\n    },\n    \"poHeaderId\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"Matched purchase order header ID\"\n    },\n    \"goodsReceivedDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Date goods were received\"\n    },\n    \"glDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"General Ledger accounting date\"\n    },\n    \"payGroupLookupCode\": {\n      \"type\": [\"string\", \"\
  null\"],\n      \"description\": \"Pay group\"\n    },\n    \"cancelledDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Date the invoice was cancelled\"\n    },\n    \"cancelledAmount\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Cancelled amount\"\n    },\n    \"lines\": {\n      \"type\": \"array\",\n      \"description\": \"Invoice lines\",\n      \"items\": {\n        \"$ref\": \"#/$defs/InvoiceLine\"\n      }\n    },\n    \"payments\": {\n      \"type\": \"array\",\n      \"description\": \"Payment records associated with this invoice\",\n      \"items\": {\n        \"$ref\": \"#/$defs/InvoicePayment\"\n      }\n    },\n    \"holds\": {\n      \"type\": \"array\",\n      \"description\": \"Active holds on this invoice\",\n      \"items\": {\n        \"$ref\": \"#/$defs/InvoiceHold\"\n      }\n    },\n    \"orgId\": {\n      \"type\": \"integer\",\n      \"description\": \"Operating unit identifier\"\
  \n    },\n    \"createdBy\": {\n      \"type\": \"integer\",\n      \"description\": \"User who created the record\"\n    },\n    \"creationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record creation date\"\n    },\n    \"lastUpdatedBy\": {\n      \"type\": \"integer\",\n      \"description\": \"User who last updated the record\"\n    },\n    \"lastUpdateDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record last update date\"\n    }\n  },\n  \"$defs\": {\n    \"InvoiceLine\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"invoiceLineId\",\n        \"lineNumber\",\n        \"lineTypeCode\",\n        \"amount\"\n      ],\n      \"properties\": {\n        \"invoiceLineId\": {\n          \"type\": \"integer\",\n          \"description\": \"Invoice line identifier\"\n        },\n        \"lineNumber\": {\n          \"type\": \"integer\",\n          \"description\": \"\
  Line number\",\n          \"minimum\": 1\n        },\n        \"lineTypeCode\": {\n          \"type\": \"string\",\n          \"description\": \"Line type\",\n          \"enum\": [\n            \"ITEM\",\n            \"TAX\",\n            \"FREIGHT\",\n            \"MISCELLANEOUS\",\n            \"PREPAY\",\n            \"AWT\",\n            \"RETAINAGE\"\n          ]\n        },\n        \"amount\": {\n          \"type\": \"number\",\n          \"description\": \"Line amount\"\n        },\n        \"baseAmount\": {\n          \"type\": [\"number\", \"null\"],\n          \"description\": \"Line amount in base currency\"\n        },\n        \"description\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Line description\",\n          \"maxLength\": 240\n        },\n        \"accountingDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"GL accounting date\"\n        },\n        \"distCodeCombinationId\"\
  : {\n          \"type\": \"integer\",\n          \"description\": \"Default distribution account code combination ID\"\n        },\n        \"itemDescription\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Item description\"\n        },\n        \"quantity\": {\n          \"type\": [\"number\", \"null\"],\n          \"description\": \"Line quantity invoiced\"\n        },\n        \"unitPrice\": {\n          \"type\": [\"number\", \"null\"],\n          \"description\": \"Unit price\"\n        },\n        \"unitMeasLookupCode\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Unit of measure\"\n        },\n        \"poHeaderId\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Matched PO header ID\"\n        },\n        \"poLineId\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Matched PO line ID\"\n        },\n        \"poLineLocationId\": {\n          \"type\": [\"\
  integer\", \"null\"],\n          \"description\": \"Matched PO shipment ID\"\n        },\n        \"poDistributionId\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Matched PO distribution ID\"\n        },\n        \"receiptNumber\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Receipt number for 3-way match\"\n        },\n        \"inventoryItemId\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Inventory item identifier\"\n        },\n        \"taxClassificationCode\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Tax classification code\"\n        },\n        \"deferredAcctgFlag\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"Y\",\n            \"N\"\n          ]\n        },\n        \"cancelledFlag\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"Y\",\n            \"N\"\n          ]\n        },\n      \
  \  \"creationDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"lastUpdateDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    },\n    \"InvoicePayment\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"invoicePaymentId\": {\n          \"type\": \"integer\",\n          \"description\": \"Invoice payment identifier\"\n        },\n        \"checkId\": {\n          \"type\": \"integer\",\n          \"description\": \"Payment check identifier\"\n        },\n        \"paymentNum\": {\n          \"type\": \"integer\",\n          \"description\": \"Payment number\"\n        },\n        \"amount\": {\n          \"type\": \"number\",\n          \"description\": \"Payment amount\"\n        },\n        \"discountTaken\": {\n          \"type\": [\"number\", \"null\"],\n          \"description\": \"Discount taken\"\n        },\n        \"accountingDate\": {\n          \"type\"\
  : \"string\",\n          \"format\": \"date\"\n        }\n      }\n    },\n    \"InvoiceHold\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"holdLookupCode\": {\n          \"type\": \"string\",\n          \"description\": \"Hold reason lookup code\"\n        },\n        \"holdReason\": {\n          \"type\": \"string\",\n          \"description\": \"Hold reason description\"\n        },\n        \"holdDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Date hold was applied\"\n        },\n        \"releaseReason\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Hold release reason\"\n        },\n        \"releaseLookupCode\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Release reason lookup code\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Hold status\",\n          \"enum\": [\n            \"ACTIVE\"\
  ,\n            \"RELEASED\"\n          ]\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/invoice.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: Oracle EBS Invoice
---
