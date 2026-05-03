---
description: A shipment managed by Ryder Transportation Management
layout: schema
name: Ryder Shipment
properties_list:
- description: Unique shipment identifier
  name: shipmentId
  type: string
- description: Current shipment status
  name: status
  type: string
- description: ''
  name: origin
  type: object
- description: ''
  name: destination
  type: object
- description: Requested pickup date
  name: requestedPickupDate
  type: string
- description: Requested delivery date
  name: requestedDeliveryDate
  type: string
- description: Actual pickup date and time
  name: actualPickupDate
  type: string
- description: Actual delivery date and time
  name: actualDeliveryDate
  type: string
- description: Total weight in pounds
  name: weight
  type: number
- description: Description of the shipment commodity
  name: commodityDescription
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: Ryder System
provider_slug: ryder-system
schema_file: json-schema/ryder-shipment-schema.json
slug: ryder-shipment
source_filename: ryder-shipment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://api-evangelist.github.io/ryder-system/json-schema/ryder-shipment-schema.json\",\n  \"title\": \"Ryder Shipment\",\n  \"description\": \"A shipment managed by Ryder Transportation Management\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"shipmentId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique shipment identifier\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"pending\", \"in_transit\", \"delivered\", \"cancelled\"],\n      \"description\": \"Current shipment status\"\n    },\n    \"origin\": {\n      \"$ref\": \"#/$defs/Address\"\n    },\n    \"destination\": {\n      \"$ref\": \"#/$defs/Address\"\n    },\n    \"requestedPickupDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Requested pickup date\"\n    },\n    \"requestedDeliveryDate\": {\n      \"type\": \"string\",\n      \"format\": \"\
  date\",\n      \"description\": \"Requested delivery date\"\n    },\n    \"actualPickupDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Actual pickup date and time\"\n    },\n    \"actualDeliveryDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Actual delivery date and time\"\n    },\n    \"weight\": {\n      \"type\": \"number\",\n      \"description\": \"Total weight in pounds\"\n    },\n    \"commodityDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the shipment commodity\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\"shipmentId\", \"status\"],\n  \"$defs\": {\n    \"Address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\"\
  \n        },\n        \"address\": {\n          \"type\": \"string\"\n        },\n        \"city\": {\n          \"type\": \"string\"\n        },\n        \"state\": {\n          \"type\": \"string\"\n        },\n        \"zip\": {\n          \"type\": \"string\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"default\": \"US\"\n        }\n      },\n      \"required\": [\"address\", \"city\", \"state\", \"zip\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/json-schema/ryder-shipment-schema.json
tags:
- Fleet Management
- Logistics
- Supply Chain
- Transportation
- Trucking
title: Ryder Shipment
---
