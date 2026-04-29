---
description: ''
layout: schema
name: PurchaseOrderShipment
properties_list:
- description: Line location (shipment) identifier
  name: lineLocationId
  type: integer
- description: Shipment number
  name: shipmentNum
  type: integer
- description: Shipment quantity
  name: quantity
  type: number
- description: Quantity received
  name: quantityReceived
  type: number
- description: Quantity billed
  name: quantityBilled
  type: number
- description: ''
  name: needByDate
  type: string
- description: ''
  name: promisedDate
  type: string
- description: Ship-to organization identifier
  name: shipToOrganizationId
  type: integer
- description: Ship-to location identifier
  name: shipToLocationId
  type: integer
- description: Shipment close status
  name: closedCode
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/supply-chain-purchase-order-shipment-schema.json
slug: supply-chain-purchase-order-shipment
source_filename: supply-chain-purchase-order-shipment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PurchaseOrderShipment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lineLocationId\": {\n      \"type\": \"integer\",\n      \"description\": \"Line location (shipment) identifier\"\n    },\n    \"shipmentNum\": {\n      \"type\": \"integer\",\n      \"description\": \"Shipment number\"\n    },\n    \"quantity\": {\n      \"type\": \"number\",\n      \"description\": \"Shipment quantity\"\n    },\n    \"quantityReceived\": {\n      \"type\": \"number\",\n      \"description\": \"Quantity received\"\n    },\n    \"quantityBilled\": {\n      \"type\": \"number\",\n      \"description\": \"Quantity billed\"\n    },\n    \"needByDate\": {\n      \"type\": \"string\"\n    },\n    \"promisedDate\": {\n      \"type\": \"string\"\n    },\n    \"shipToOrganizationId\": {\n      \"type\": \"integer\",\n      \"description\": \"Ship-to organization identifier\"\n    },\n    \"shipToLocationId\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Ship-to location identifier\"\n    },\n    \"closedCode\": {\n      \"type\": \"string\",\n      \"description\": \"Shipment close status\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/supply-chain-purchase-order-shipment-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: PurchaseOrderShipment
---
