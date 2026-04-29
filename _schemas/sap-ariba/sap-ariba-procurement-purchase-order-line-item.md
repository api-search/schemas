---
description: A line item within a purchase order representing a specific good or service being procured
layout: schema
name: PurchaseOrderLineItem
properties_list:
- description: Line item number within the purchase order. Unique within the order.
  name: numberOnPO
  type: string
- description: Description of the item or service being purchased
  name: description
  type: string
- description: Quantity to purchase
  name: quantity
  type: number
- description: Buyer-assigned part or material number
  name: buyerPartNumber
  type: string
- description: Supplier-assigned part or catalog number
  name: supplierPartNumber
  type: string
- description: Manufacturer part identifier
  name: manufacturerPartId
  type: string
- description: Name of the manufacturer
  name: manufacturerName
  type: string
- description: Item category code distinguishing material, service, or other item types
  name: itemCategory
  type: string
- description: Account assignment category for the line item expenditure
  name: accountCategory
  type: string
- description: Requested delivery date for the line item (ISO 8601 YYYY-MM-DD)
  name: needByDate
  type: string
- description: Split accounting assignments for distributing costs across multiple cost objects
  name: accountings
  type: array
- description: Receiving type value indicating how receipts should be processed for this line item
  name: receivingType
  type: integer
- description: Tax code per evaluated receipt settlement agreements
  name: taxCode
  type: string
- description: Line number of the corresponding item in the originating requisition
  name: itemOnRequisition
  type: string
- description: Service period start date (for service line items)
  name: serviceStartDate
  type: string
- description: Service period end date (for service line items)
  name: serviceEndDate
  type: string
- description: Additional comments or notes on the line item
  name: comments
  type: string
provider_name: SAP Ariba
provider_slug: sap-ariba
schema_file: json-schema/sap-ariba-procurement-purchase-order-line-item-schema.json
slug: sap-ariba-procurement-purchase-order-line-item
source_filename: sap-ariba-procurement-purchase-order-line-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PurchaseOrderLineItem\",\n  \"type\": \"object\",\n  \"description\": \"A line item within a purchase order representing a specific good or service being procured\",\n  \"properties\": {\n    \"numberOnPO\": {\n      \"type\": \"string\",\n      \"description\": \"Line item number within the purchase order. Unique within the order.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the item or service being purchased\"\n    },\n    \"quantity\": {\n      \"type\": \"number\",\n      \"description\": \"Quantity to purchase\"\n    },\n    \"buyerPartNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Buyer-assigned part or material number\"\n    },\n    \"supplierPartNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Supplier-assigned part or catalog number\"\n    },\n    \"manufacturerPartId\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Manufacturer part identifier\"\n    },\n    \"manufacturerName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the manufacturer\"\n    },\n    \"itemCategory\": {\n      \"type\": \"string\",\n      \"description\": \"Item category code distinguishing material, service, or other item types\"\n    },\n    \"accountCategory\": {\n      \"type\": \"string\",\n      \"description\": \"Account assignment category for the line item expenditure\"\n    },\n    \"needByDate\": {\n      \"type\": \"string\",\n      \"description\": \"Requested delivery date for the line item (ISO 8601 YYYY-MM-DD)\"\n    },\n    \"accountings\": {\n      \"type\": \"array\",\n      \"description\": \"Split accounting assignments for distributing costs across multiple cost objects\"\n    },\n    \"receivingType\": {\n      \"type\": \"integer\",\n      \"description\": \"Receiving type value indicating how receipts should be processed for this line item\"\
  \n    },\n    \"taxCode\": {\n      \"type\": \"string\",\n      \"description\": \"Tax code per evaluated receipt settlement agreements\"\n    },\n    \"itemOnRequisition\": {\n      \"type\": \"string\",\n      \"description\": \"Line number of the corresponding item in the originating requisition\"\n    },\n    \"serviceStartDate\": {\n      \"type\": \"string\",\n      \"description\": \"Service period start date (for service line items)\"\n    },\n    \"serviceEndDate\": {\n      \"type\": \"string\",\n      \"description\": \"Service period end date (for service line items)\"\n    },\n    \"comments\": {\n      \"type\": \"string\",\n      \"description\": \"Additional comments or notes on the line item\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/json-schema/sap-ariba-procurement-purchase-order-line-item-schema.json
tags:
- B2B
- Contract Management
- Procurement
- Sourcing
- Spend Analysis
- Supplier Management
- Supply Chain
title: PurchaseOrderLineItem
---
