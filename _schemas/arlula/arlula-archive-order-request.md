---
description: Request body for ordering archive imagery.
layout: schema
name: ArchiveOrderRequest
properties_list:
- description: Ordering ID of the archive scene to purchase.
  name: id
  type: string
- description: Bundle key selected from search results.
  name: bundleKey
  type: string
- description: EULA identifier accepted for this order.
  name: eula
  type: string
- description: ''
  name: emails
  type: array
- description: ''
  name: webhooks
  type: array
- description: Optional coupon code for discounts.
  name: coupon
  type: string
provider_name: Arlula
provider_slug: arlula
schema_file: json-schema/arlula-archive-order-request-schema.json
slug: arlula-archive-order-request
source_filename: arlula-archive-order-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://arlula.com/json-schema/archive-order-request.json\",\n  \"title\": \"ArchiveOrderRequest\",\n  \"description\": \"Request body for ordering archive imagery.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Ordering ID of the archive scene to purchase.\",\n      \"examples\": [\n        \"a1b2c3d4-e5f6-7890-abcd-ef1234567890\"\n      ]\n    },\n    \"bundleKey\": {\n      \"type\": \"string\",\n      \"description\": \"Bundle key selected from search results.\",\n      \"examples\": [\n        \"bundle-basic\"\n      ]\n    },\n    \"eula\": {\n      \"type\": \"string\",\n      \"description\": \"EULA identifier accepted for this order.\",\n      \"examples\": [\n        \"EULA-001\"\n      ]\n    },\n    \"emails\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n  \
  \  \"webhooks\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"coupon\": {\n      \"type\": \"string\",\n      \"description\": \"Optional coupon code for discounts.\",\n      \"examples\": [\n        \"COUPON-001\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arlula/refs/heads/main/json-schema/arlula-archive-order-request-schema.json
tags:
- Earth Observation
- Geospatial
- Imagery
- Remote Sensing
- Satellites
title: ArchiveOrderRequest
---
