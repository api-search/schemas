---
description: InventorySummaries schema from Amazon Selling Partner API
layout: schema
name: InventorySummaries
properties_list:
- description: ''
  name: pagination
  type: object
- description: ''
  name: inventorySummaries
  type: array
provider_name: Amazon
provider_slug: amazon
schema_file: json-schema/selling-partner-inventory-summaries-schema.json
slug: selling-partner-inventory-summaries
source_filename: selling-partner-inventory-summaries-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"pagination\": {\n      \"$ref\": \"#/components/schemas/Pagination\"\n    },\n    \"inventorySummaries\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"asin\": {\n            \"type\": \"string\"\n          },\n          \"fnSku\": {\n            \"type\": \"string\"\n          },\n          \"sellerSku\": {\n            \"type\": \"string\"\n          },\n          \"condition\": {\n            \"type\": \"string\"\n          },\n          \"inventoryDetails\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"fulfillableQuantity\": {\n                \"type\": \"integer\"\n              },\n              \"inboundWorkingQuantity\": {\n                \"type\": \"integer\"\n              },\n              \"inboundShippedQuantity\": {\n                \"type\": \"integer\"\n              },\n              \"inboundReceivingQuantity\"\
  : {\n                \"type\": \"integer\"\n              },\n              \"reservedQuantity\": {\n                \"type\": \"object\"\n              },\n              \"unfulfillableQuantity\": {\n                \"type\": \"object\"\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InventorySummaries\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/selling-partner-inventory-summaries-schema.json\",\n  \"description\": \"InventorySummaries schema from Amazon Selling Partner API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/selling-partner-inventory-summaries-schema.json
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
title: InventorySummaries
---
