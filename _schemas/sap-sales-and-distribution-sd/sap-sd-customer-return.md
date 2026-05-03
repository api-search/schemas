---
description: Schema for SAP S/4HANA Customer Return entity (A_CustomerReturn) from the API_CREDIT_MEMO_REQUEST_SRV OData service. Represents a customer return document used to process returned goods in reverse logistics.
layout: schema
name: SAP Customer Return
properties_list:
- description: Customer return number
  name: CustomerReturn
  type: string
- description: Sales document type
  name: CustomerReturnType
  type: string
- description: Sales organization
  name: SalesOrganization
  type: string
- description: Distribution channel
  name: DistributionChannel
  type: string
- description: Division
  name: OrganizationDivision
  type: string
- description: Sold-to party
  name: SoldToParty
  type: string
- description: Creation date
  name: CreationDate
  type: string
- description: Document date
  name: CustomerReturnDate
  type: string
- description: Net value in document currency
  name: TotalNetAmount
  type: string
- description: Document currency
  name: TransactionCurrency
  type: string
- description: Return reason
  name: SDDocumentReason
  type: string
- description: Overall processing status
  name: OverallSDProcessStatus
  type: string
- description: Delivery status
  name: OverallDeliveryStatus
  type: string
- description: Billing status
  name: OverallBillingStatus
  type: string
provider_name: SAP Sales and Distribution (SD)
provider_slug: sap-sales-and-distribution-sd
schema_file: json-schema/sap-sd-customer-return-schema.json
slug: sap-sd-customer-return
source_filename: sap-sd-customer-return-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.sap.com/schemas/sap-sd-customer-return\",\n  \"title\": \"SAP Customer Return\",\n  \"description\": \"Schema for SAP S/4HANA Customer Return entity (A_CustomerReturn) from the API_CREDIT_MEMO_REQUEST_SRV OData service. Represents a customer return document used to process returned goods in reverse logistics.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CustomerReturn\": {\n      \"type\": \"string\",\n      \"maxLength\": 10,\n      \"description\": \"Customer return number\"\n    },\n    \"CustomerReturnType\": {\n      \"type\": \"string\",\n      \"maxLength\": 4,\n      \"description\": \"Sales document type\"\n    },\n    \"SalesOrganization\": {\n      \"type\": \"string\",\n      \"maxLength\": 4,\n      \"description\": \"Sales organization\"\n    },\n    \"DistributionChannel\": {\n      \"type\": \"string\",\n      \"maxLength\": 2,\n      \"description\": \"\
  Distribution channel\"\n    },\n    \"OrganizationDivision\": {\n      \"type\": \"string\",\n      \"maxLength\": 2,\n      \"description\": \"Division\"\n    },\n    \"SoldToParty\": {\n      \"type\": \"string\",\n      \"maxLength\": 10,\n      \"description\": \"Sold-to party\"\n    },\n    \"CreationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Creation date\"\n    },\n    \"CustomerReturnDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Document date\"\n    },\n    \"TotalNetAmount\": {\n      \"type\": \"string\",\n      \"description\": \"Net value in document currency\"\n    },\n    \"TransactionCurrency\": {\n      \"type\": \"string\",\n      \"maxLength\": 5,\n      \"description\": \"Document currency\"\n    },\n    \"SDDocumentReason\": {\n      \"type\": \"string\",\n      \"maxLength\": 3,\n      \"description\": \"Return reason\"\n    },\n    \"OverallSDProcessStatus\": {\n   \
  \   \"type\": \"string\",\n      \"maxLength\": 1,\n      \"description\": \"Overall processing status\"\n    },\n    \"OverallDeliveryStatus\": {\n      \"type\": \"string\",\n      \"maxLength\": 1,\n      \"description\": \"Delivery status\"\n    },\n    \"OverallBillingStatus\": {\n      \"type\": \"string\",\n      \"maxLength\": 1,\n      \"description\": \"Billing status\"\n    }\n  },\n  \"required\": [\"CustomerReturn\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/json-schema/sap-sd-customer-return-schema.json
tags:
- Distribution
- ERP
- OData
- S/4HANA
- Sales
- SAP
title: SAP Customer Return
---
