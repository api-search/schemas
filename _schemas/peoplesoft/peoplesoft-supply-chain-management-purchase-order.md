---
description: PeopleSoft purchasing purchase order.
layout: schema
name: PurchaseOrder
properties_list:
- description: Business unit.
  name: BUSINESS_UNIT
  type: string
- description: Purchase order ID.
  name: PO_ID
  type: string
- description: Vendor ID.
  name: VENDOR_ID
  type: string
- description: PO date.
  name: PO_DT
  type: string
- description: PO status.
  name: PO_STATUS
  type: string
- description: Currency.
  name: CURRENCY_CD
  type: string
- description: Buyer ID.
  name: BUYER_ID
  type: string
- description: Ship-to location.
  name: SHIP_TO_LOCATION
  type: string
- description: PO lines.
  name: LINES
  type: array
provider_name: PeopleSoft
provider_slug: peoplesoft
schema_file: json-schema/peoplesoft-supply-chain-management-purchase-order-schema.json
slug: peoplesoft-supply-chain-management-purchase-order
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/json-schema/peoplesoft-supply-chain-management-purchase-order-schema.json\",\n  \"title\": \"PurchaseOrder\",\n  \"description\": \"PeopleSoft purchasing purchase order.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BUSINESS_UNIT\": {\n      \"type\": \"string\",\n      \"description\": \"Business unit.\",\n      \"example\": \"US001\"\n    },\n    \"PO_ID\": {\n      \"type\": \"string\",\n      \"description\": \"Purchase order ID.\",\n      \"example\": \"PO0012345\"\n    },\n    \"VENDOR_ID\": {\n      \"type\": \"string\",\n      \"description\": \"Vendor ID.\",\n      \"example\": \"VND001234\"\n    },\n    \"PO_DT\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"PO date.\",\n      \"example\": \"2026-04-17\"\n    },\n    \"PO_STATUS\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"PO status.\",\n      \"enum\": [\n        \"O\",\n        \"A\",\n        \"C\",\n        \"D\",\n        \"X\",\n        \"PX\"\n      ],\n      \"example\": \"A\"\n    },\n    \"CURRENCY_CD\": {\n      \"type\": \"string\",\n      \"description\": \"Currency.\",\n      \"example\": \"USD\"\n    },\n    \"BUYER_ID\": {\n      \"type\": \"string\",\n      \"description\": \"Buyer ID.\",\n      \"example\": \"BYR001\"\n    },\n    \"SHIP_TO_LOCATION\": {\n      \"type\": \"string\",\n      \"description\": \"Ship-to location.\",\n      \"example\": \"WH001\"\n    },\n    \"LINES\": {\n      \"type\": \"array\",\n      \"description\": \"PO lines.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"LINE_NBR\": {\n            \"type\": \"integer\",\n            \"description\": \"Line number.\",\n            \"example\": 1\n          },\n          \"INV_ITEM_ID\": {\n            \"type\": \"string\",\n            \"description\"\
  : \"Item ID.\",\n            \"example\": \"ITEM001234\"\n          },\n          \"DESCR\": {\n            \"type\": \"string\",\n            \"description\": \"Description.\",\n            \"example\": \"Office Chair - Ergonomic\"\n          },\n          \"QTY_PO\": {\n            \"type\": \"number\",\n            \"description\": \"Quantity.\",\n            \"example\": 25\n          },\n          \"PRICE_PO\": {\n            \"type\": \"number\",\n            \"description\": \"Unit price.\",\n            \"example\": 450.0\n          },\n          \"UNIT_OF_MEASURE\": {\n            \"type\": \"string\",\n            \"description\": \"UOM.\",\n            \"example\": \"EA\"\n          }\n        }\n      }\n    }\n  },\n  \"x-schema-source\": \"domain-knowledge\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/json-schema/peoplesoft-supply-chain-management-purchase-order-schema.json
tags:
- Campus Solutions
- CRM
- Enterprise Software
- ERP
- Financial Management
- HCM
- Supply Chain Management
title: PurchaseOrder
---
