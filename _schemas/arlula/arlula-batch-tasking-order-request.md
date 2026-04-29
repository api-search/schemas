---
description: Request body for placing multiple tasking orders simultaneously.
layout: schema
name: BatchTaskingOrderRequest
properties_list:
- description: ''
  name: orders
  type: array
- description: ''
  name: emails
  type: array
provider_name: Arlula
provider_slug: arlula
schema_file: json-schema/arlula-batch-tasking-order-request-schema.json
slug: arlula-batch-tasking-order-request
source_filename: arlula-batch-tasking-order-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://arlula.com/json-schema/batch-tasking-order-request.json\",\n  \"title\": \"BatchTaskingOrderRequest\",\n  \"description\": \"Request body for placing multiple tasking orders simultaneously.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"orders\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"https://arlula.com/json-schema/tasking-order-request.json\"\n      }\n    },\n    \"emails\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arlula/refs/heads/main/json-schema/arlula-batch-tasking-order-request-schema.json
tags:
- Earth Observation
- Geospatial
- Imagery
- Remote Sensing
- Satellites
title: BatchTaskingOrderRequest
---
