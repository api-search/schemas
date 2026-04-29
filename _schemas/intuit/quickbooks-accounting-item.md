---
description: An Item represents a product or service that a company buys, sells, or re-sells. Items are used in line items on invoices, sales receipts, bills, and other transactions.
layout: schema
name: Item
properties_list:
- description: Unique identifier for the item
  name: Id
  type: string
- description: Version number for optimistic locking
  name: SyncToken
  type: string
- description: Name of the item. Must be unique within the same type.
  name: Name
  type: string
- description: Description of the item used in sales transactions
  name: Description
  type: string
- description: Description of the item used in purchase transactions
  name: PurchaseDesc
  type: string
- description: Whether the item is currently active
  name: Active
  type: boolean
- description: Fully qualified name of the item
  name: FullyQualifiedName
  type: string
- description: Whether sales of this item are taxable
  name: Taxable
  type: boolean
- description: Whether the sales tax is included in the item amount
  name: SalesTaxIncluded
  type: boolean
- description: Sales price for this item
  name: UnitPrice
  type: number
- description: Classification of the item
  name: Type
  type: string
- description: Purchase cost of the item
  name: PurchaseCost
  type: number
- description: Current quantity on hand (inventory items only)
  name: QtyOnHand
  type: number
- description: Date of opening balance for inventory items
  name: InvStartDate
  type: string
- description: Whether quantity on hand is tracked
  name: TrackQtyOnHand
  type: boolean
- description: Stock keeping unit identifier
  name: Sku
  type: string
- description: Whether this is a sub-item
  name: SubItem
  type: boolean
- description: Depth level in the item hierarchy
  name: Level
  type: integer
- description: ''
  name: AbatementRate
  type: number
- description: ''
  name: ReverseChargeRate
  type: number
- description: ''
  name: domain
  type: string
- description: ''
  name: sparse
  type: boolean
provider_name: Intuit
provider_slug: intuit
schema_file: json-schema/quickbooks-accounting-item-schema.json
slug: quickbooks-accounting-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Item\",\n  \"type\": \"object\",\n  \"description\": \"An Item represents a product or service that a company buys, sells, or re-sells. Items are used in line items on invoices, sales receipts, bills, and other transactions.\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the item\"\n    },\n    \"SyncToken\": {\n      \"type\": \"string\",\n      \"description\": \"Version number for optimistic locking\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the item. Must be unique within the same type.\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the item used in sales transactions\"\n    },\n    \"PurchaseDesc\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the item used in purchase transactions\"\n    },\n\
  \    \"Active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the item is currently active\"\n    },\n    \"FullyQualifiedName\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified name of the item\"\n    },\n    \"Taxable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether sales of this item are taxable\"\n    },\n    \"SalesTaxIncluded\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the sales tax is included in the item amount\"\n    },\n    \"UnitPrice\": {\n      \"type\": \"number\",\n      \"description\": \"Sales price for this item\"\n    },\n    \"Type\": {\n      \"type\": \"string\",\n      \"description\": \"Classification of the item\"\n    },\n    \"PurchaseCost\": {\n      \"type\": \"number\",\n      \"description\": \"Purchase cost of the item\"\n    },\n    \"QtyOnHand\": {\n      \"type\": \"number\",\n      \"description\": \"Current quantity on hand (inventory items only)\"\n    },\n \
  \   \"InvStartDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date of opening balance for inventory items\"\n    },\n    \"TrackQtyOnHand\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether quantity on hand is tracked\"\n    },\n    \"Sku\": {\n      \"type\": \"string\",\n      \"description\": \"Stock keeping unit identifier\"\n    },\n    \"SubItem\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a sub-item\"\n    },\n    \"Level\": {\n      \"type\": \"integer\",\n      \"description\": \"Depth level in the item hierarchy\"\n    },\n    \"AbatementRate\": {\n      \"type\": \"number\"\n    },\n    \"ReverseChargeRate\": {\n      \"type\": \"number\"\n    },\n    \"domain\": {\n      \"type\": \"string\"\n    },\n    \"sparse\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/intuit/refs/heads/main/json-schema/quickbooks-accounting-item-schema.json
tags:
- Accounting
- Custom Fields
- Financial
- Financial Services
- Invoicing
- Payments
- Payroll
- Project Management
- Sales Tax
- Small Business
- Tax
- Tax Preparation
- Taxes
- Time Tracking
title: Item
---
