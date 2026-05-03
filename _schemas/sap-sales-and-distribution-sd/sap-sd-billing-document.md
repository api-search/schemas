---
description: Schema for SAP S/4HANA Billing Document entity (A_BillingDocument) from the API_BILLING_DOCUMENT_SRV OData service. Represents billing document headers including invoices, credit memos, and debit memos.
layout: schema
name: SAP Billing Document
properties_list:
- description: Billing document number
  name: BillingDocument
  type: string
- description: Billing document type (F2=Invoice, G2=Credit Memo, L2=Debit Memo)
  name: BillingDocumentType
  type: string
- description: Billing document category
  name: BillingDocumentCategory
  type: string
- description: SD document category
  name: SDDocumentCategory
  type: string
- description: Billing date
  name: BillingDocumentDate
  type: string
- description: Date the document was created
  name: CreationDate
  type: string
- description: Date of last change
  name: LastChangeDate
  type: string
- description: Sales organization
  name: SalesOrganization
  type: string
- description: Distribution channel
  name: DistributionChannel
  type: string
- description: Division
  name: Division
  type: string
- description: Sold-to party
  name: SoldToParty
  type: string
- description: Payer
  name: PayerParty
  type: string
- description: Net value in document currency
  name: TotalNetAmount
  type: string
- description: Gross value in document currency
  name: TotalGrossAmount
  type: string
- description: SD document currency
  name: TransactionCurrency
  type: string
- description: Tax amount in document currency
  name: TotalTaxAmount
  type: string
- description: Indicates if the billing document is cancelled
  name: BillingDocumentIsCancelled
  type: boolean
- description: Cancelled billing document number
  name: CancelledBillingDocument
  type: string
- description: Accounting document number
  name: AccountingDocument
  type: string
- description: Company code
  name: CompanyCode
  type: string
provider_name: SAP Sales and Distribution (SD)
provider_slug: sap-sales-and-distribution-sd
schema_file: json-schema/sap-sd-billing-document-schema.json
slug: sap-sd-billing-document
source_filename: sap-sd-billing-document-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.sap.com/schemas/sap-sd-billing-document\",\n  \"title\": \"SAP Billing Document\",\n  \"description\": \"Schema for SAP S/4HANA Billing Document entity (A_BillingDocument) from the API_BILLING_DOCUMENT_SRV OData service. Represents billing document headers including invoices, credit memos, and debit memos.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BillingDocument\": {\n      \"type\": \"string\",\n      \"maxLength\": 10,\n      \"description\": \"Billing document number\"\n    },\n    \"BillingDocumentType\": {\n      \"type\": \"string\",\n      \"maxLength\": 4,\n      \"description\": \"Billing document type (F2=Invoice, G2=Credit Memo, L2=Debit Memo)\"\n    },\n    \"BillingDocumentCategory\": {\n      \"type\": \"string\",\n      \"maxLength\": 1,\n      \"description\": \"Billing document category\"\n    },\n    \"SDDocumentCategory\": {\n      \"type\": \"string\"\
  ,\n      \"maxLength\": 4,\n      \"description\": \"SD document category\"\n    },\n    \"BillingDocumentDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Billing date\"\n    },\n    \"CreationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the document was created\"\n    },\n    \"LastChangeDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of last change\"\n    },\n    \"SalesOrganization\": {\n      \"type\": \"string\",\n      \"maxLength\": 4,\n      \"description\": \"Sales organization\"\n    },\n    \"DistributionChannel\": {\n      \"type\": \"string\",\n      \"maxLength\": 2,\n      \"description\": \"Distribution channel\"\n    },\n    \"Division\": {\n      \"type\": \"string\",\n      \"maxLength\": 2,\n      \"description\": \"Division\"\n    },\n    \"SoldToParty\": {\n      \"type\": \"string\",\n      \"maxLength\": 10,\n    \
  \  \"description\": \"Sold-to party\"\n    },\n    \"PayerParty\": {\n      \"type\": \"string\",\n      \"maxLength\": 10,\n      \"description\": \"Payer\"\n    },\n    \"TotalNetAmount\": {\n      \"type\": \"string\",\n      \"description\": \"Net value in document currency\"\n    },\n    \"TotalGrossAmount\": {\n      \"type\": \"string\",\n      \"description\": \"Gross value in document currency\"\n    },\n    \"TransactionCurrency\": {\n      \"type\": \"string\",\n      \"maxLength\": 5,\n      \"description\": \"SD document currency\"\n    },\n    \"TotalTaxAmount\": {\n      \"type\": \"string\",\n      \"description\": \"Tax amount in document currency\"\n    },\n    \"BillingDocumentIsCancelled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates if the billing document is cancelled\"\n    },\n    \"CancelledBillingDocument\": {\n      \"type\": \"string\",\n      \"maxLength\": 10,\n      \"description\": \"Cancelled billing document number\"\n    },\n \
  \   \"AccountingDocument\": {\n      \"type\": \"string\",\n      \"maxLength\": 10,\n      \"description\": \"Accounting document number\"\n    },\n    \"CompanyCode\": {\n      \"type\": \"string\",\n      \"maxLength\": 4,\n      \"description\": \"Company code\"\n    }\n  },\n  \"required\": [\"BillingDocument\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/json-schema/sap-sd-billing-document-schema.json
tags:
- Distribution
- ERP
- OData
- S/4HANA
- Sales
- SAP
title: SAP Billing Document
---
