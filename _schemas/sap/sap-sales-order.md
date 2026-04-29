---
description: Schema for SAP sales order documents used in S/4HANA and Business One APIs.
layout: schema
name: SAP Sales Order
properties_list:
- description: Sales order number
  name: SalesOrder
  type: string
- description: Sales document type
  name: SalesOrderType
  type: string
- description: Sales organization code
  name: SalesOrganization
  type: string
- description: Distribution channel
  name: DistributionChannel
  type: string
- description: Division
  name: OrganizationDivision
  type: string
- description: Sold-to party business partner number
  name: SoldToParty
  type: string
- description: Customer purchase order number
  name: PurchaseOrderByCustomer
  type: string
- description: Sales order date
  name: SalesOrderDate
  type: string
- description: Requested delivery date
  name: RequestedDeliveryDate
  type: string
- description: Net value of the sales order in document currency
  name: TotalNetAmount
  type: number
- description: Document currency (ISO 4217)
  name: TransactionCurrency
  type: string
- description: Overall delivery status
  name: OverallDeliveryStatus
  type: string
- description: Sales order line items
  name: Items
  type: array
provider_name: SAP
provider_slug: sap
schema_file: json-schema/sap-sales-order-schema.json
slug: sap-sales-order
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.sap.com/schemas/sap/sales-order.json\",\n  \"title\": \"SAP Sales Order\",\n  \"description\": \"Schema for SAP sales order documents used in S/4HANA and Business One APIs.\",\n  \"type\": \"object\",\n  \"required\": [\"SalesOrderType\", \"SoldToParty\"],\n  \"properties\": {\n    \"SalesOrder\": {\n      \"type\": \"string\",\n      \"description\": \"Sales order number\",\n      \"maxLength\": 10,\n      \"readOnly\": true\n    },\n    \"SalesOrderType\": {\n      \"type\": \"string\",\n      \"description\": \"Sales document type\",\n      \"maxLength\": 4\n    },\n    \"SalesOrganization\": {\n      \"type\": \"string\",\n      \"description\": \"Sales organization code\",\n      \"maxLength\": 4\n    },\n    \"DistributionChannel\": {\n      \"type\": \"string\",\n      \"description\": \"Distribution channel\",\n      \"maxLength\": 2\n    },\n    \"OrganizationDivision\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"Division\",\n      \"maxLength\": 2\n    },\n    \"SoldToParty\": {\n      \"type\": \"string\",\n      \"description\": \"Sold-to party business partner number\",\n      \"maxLength\": 10\n    },\n    \"PurchaseOrderByCustomer\": {\n      \"type\": \"string\",\n      \"description\": \"Customer purchase order number\",\n      \"maxLength\": 35\n    },\n    \"SalesOrderDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Sales order date\"\n    },\n    \"RequestedDeliveryDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Requested delivery date\"\n    },\n    \"TotalNetAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Net value of the sales order in document currency\"\n    },\n    \"TransactionCurrency\": {\n      \"type\": \"string\",\n      \"description\": \"Document currency (ISO 4217)\",\n      \"maxLength\": 3,\n      \"pattern\"\
  : \"^[A-Z]{3}$\"\n    },\n    \"OverallDeliveryStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Overall delivery status\",\n      \"enum\": [\"\", \"A\", \"B\", \"C\"]\n    },\n    \"Items\": {\n      \"type\": \"array\",\n      \"description\": \"Sales order line items\",\n      \"items\": {\n        \"$ref\": \"#/$defs/SalesOrderItem\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"SalesOrderItem\": {\n      \"type\": \"object\",\n      \"description\": \"Sales order line item\",\n      \"required\": [\"Material\", \"OrderQuantity\"],\n      \"properties\": {\n        \"SalesOrderItem\": {\n          \"type\": \"string\",\n          \"description\": \"Item number within the sales order\",\n          \"maxLength\": 6\n        },\n        \"Material\": {\n          \"type\": \"string\",\n          \"description\": \"Material number\",\n          \"maxLength\": 40\n        },\n        \"SalesOrderItemText\": {\n          \"type\": \"string\",\n          \"description\":\
  \ \"Item description\",\n          \"maxLength\": 40\n        },\n        \"OrderQuantity\": {\n          \"type\": \"number\",\n          \"description\": \"Order quantity\",\n          \"minimum\": 0\n        },\n        \"OrderQuantityUnit\": {\n          \"type\": \"string\",\n          \"description\": \"Unit of measure for the order quantity\",\n          \"maxLength\": 3\n        },\n        \"NetAmount\": {\n          \"type\": \"number\",\n          \"description\": \"Net value of the line item\"\n        },\n        \"Plant\": {\n          \"type\": \"string\",\n          \"description\": \"Delivering plant\",\n          \"maxLength\": 4\n        },\n        \"StorageLocation\": {\n          \"type\": \"string\",\n          \"description\": \"Storage location\",\n          \"maxLength\": 4\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/json-schema/sap-sales-order-schema.json
tags:
- AI
- BTP
- Business Applications
- Cloud
- Data Management
- Enterprise
- ERP
- Integration
title: SAP Sales Order
---
