---
description: Request payload for creating a new sales order with optional deep insert
layout: schema
name: SalesOrderCreate
properties_list:
- description: Sales document type
  name: SalesOrderType
  type: string
- description: Sales organization
  name: SalesOrganization
  type: string
- description: Distribution channel
  name: DistributionChannel
  type: string
- description: Organization division
  name: OrganizationDivision
  type: string
- description: Sold-to party customer number
  name: SoldToParty
  type: string
- description: Customer purchase order number
  name: PurchaseOrderByCustomer
  type: string
- description: Document date
  name: SalesOrderDate
  type: string
- description: Requested delivery date
  name: RequestedDeliveryDate
  type: string
- description: Payment terms key
  name: CustomerPaymentTerms
  type: string
- description: Currency key (ISO 4217)
  name: TransactionCurrency
  type: string
- description: Pricing date
  name: PricingDate
  type: string
- description: Incoterms classification
  name: IncotermsClassification
  type: string
- description: Incoterms location
  name: IncotermsTransferLocation
  type: string
- description: Shipping condition
  name: ShippingCondition
  type: string
- description: Complete delivery indicator
  name: CompleteDeliveryIsDefined
  type: boolean
- description: Order reason
  name: SDDocumentReason
  type: string
- description: Items to create (deep insert)
  name: to_Item
  type: array
- description: Partners to create (deep insert)
  name: to_Partner
  type: array
- description: Pricing elements to create (deep insert)
  name: to_PricingElement
  type: array
- description: Text records to create (deep insert)
  name: to_Text
  type: array
provider_name: SAP S/4HANA
provider_slug: sap-s4hana
schema_file: json-schema/sap-s4hana-sales-order-sales-order-create-schema.json
slug: sap-s4hana-sales-order-sales-order-create
source_filename: sap-s4hana-sales-order-sales-order-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SalesOrderCreate\",\n  \"type\": \"object\",\n  \"description\": \"Request payload for creating a new sales order with optional deep insert\",\n  \"properties\": {\n    \"SalesOrderType\": {\n      \"type\": \"string\",\n      \"description\": \"Sales document type\"\n    },\n    \"SalesOrganization\": {\n      \"type\": \"string\",\n      \"description\": \"Sales organization\"\n    },\n    \"DistributionChannel\": {\n      \"type\": \"string\",\n      \"description\": \"Distribution channel\"\n    },\n    \"OrganizationDivision\": {\n      \"type\": \"string\",\n      \"description\": \"Organization division\"\n    },\n    \"SoldToParty\": {\n      \"type\": \"string\",\n      \"description\": \"Sold-to party customer number\"\n    },\n    \"PurchaseOrderByCustomer\": {\n      \"type\": \"string\",\n      \"description\": \"Customer purchase order number\"\n    },\n    \"SalesOrderDate\":\
  \ {\n      \"type\": \"string\",\n      \"description\": \"Document date\"\n    },\n    \"RequestedDeliveryDate\": {\n      \"type\": \"string\",\n      \"description\": \"Requested delivery date\"\n    },\n    \"CustomerPaymentTerms\": {\n      \"type\": \"string\",\n      \"description\": \"Payment terms key\"\n    },\n    \"TransactionCurrency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency key (ISO 4217)\"\n    },\n    \"PricingDate\": {\n      \"type\": \"string\",\n      \"description\": \"Pricing date\"\n    },\n    \"IncotermsClassification\": {\n      \"type\": \"string\",\n      \"description\": \"Incoterms classification\"\n    },\n    \"IncotermsTransferLocation\": {\n      \"type\": \"string\",\n      \"description\": \"Incoterms location\"\n    },\n    \"ShippingCondition\": {\n      \"type\": \"string\",\n      \"description\": \"Shipping condition\"\n    },\n    \"CompleteDeliveryIsDefined\": {\n      \"type\": \"boolean\",\n      \"description\": \"\
  Complete delivery indicator\"\n    },\n    \"SDDocumentReason\": {\n      \"type\": \"string\",\n      \"description\": \"Order reason\"\n    },\n    \"to_Item\": {\n      \"type\": \"array\",\n      \"description\": \"Items to create (deep insert)\"\n    },\n    \"to_Partner\": {\n      \"type\": \"array\",\n      \"description\": \"Partners to create (deep insert)\"\n    },\n    \"to_PricingElement\": {\n      \"type\": \"array\",\n      \"description\": \"Pricing elements to create (deep insert)\"\n    },\n    \"to_Text\": {\n      \"type\": \"array\",\n      \"description\": \"Text records to create (deep insert)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/json-schema/sap-s4hana-sales-order-sales-order-create-schema.json
tags:
- Business Applications
- Cloud
- Enterprise Resource Planning
- ERP
- Finance
- Human Resources
- Inventory
- Logistics
- Manufacturing
- Plant Maintenance
- Procurement
- S/4HANA
- Sales
- SAP
title: SalesOrderCreate
---
