---
description: Request body for ordering a future satellite capture.
layout: schema
name: TaskingOrderRequest
properties_list:
- description: Ordering ID of the tasking opportunity.
  name: id
  type: string
- description: Bundle key for this order.
  name: bundleKey
  type: string
- description: EULA identifier.
  name: eula
  type: string
- description: Maximum acceptable cloud cover percentage.
  name: cloud
  type: integer
- description: Priority level for the capture.
  name: priorityKey
  type: string
- description: ''
  name: emails
  type: array
- description: ''
  name: webhooks
  type: array
- description: Optional coupon code.
  name: coupon
  type: string
provider_name: Arlula
provider_slug: arlula
schema_file: json-schema/arlula-tasking-order-request-schema.json
slug: arlula-tasking-order-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://arlula.com/json-schema/tasking-order-request.json\",\n  \"title\": \"TaskingOrderRequest\",\n  \"description\": \"Request body for ordering a future satellite capture.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Ordering ID of the tasking opportunity.\",\n      \"examples\": [\n        \"opp-a1b2c3d4\"\n      ]\n    },\n    \"bundleKey\": {\n      \"type\": \"string\",\n      \"description\": \"Bundle key for this order.\",\n      \"examples\": [\n        \"bundle-standard\"\n      ]\n    },\n    \"eula\": {\n      \"type\": \"string\",\n      \"description\": \"EULA identifier.\",\n      \"examples\": [\n        \"EULA-001\"\n      ]\n    },\n    \"cloud\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum acceptable cloud cover percentage.\",\n      \"examples\": [\n        20\n      ]\n    },\n\
  \    \"priorityKey\": {\n      \"type\": \"string\",\n      \"description\": \"Priority level for the capture.\",\n      \"examples\": [\n        \"standard\"\n      ]\n    },\n    \"emails\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"webhooks\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"coupon\": {\n      \"type\": \"string\",\n      \"description\": \"Optional coupon code.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arlula/refs/heads/main/json-schema/arlula-tasking-order-request-schema.json
tags:
- Earth Observation
- Geospatial
- Imagery
- Remote Sensing
- Satellites
title: TaskingOrderRequest
---
