---
description: Request body for updating a service price.
layout: schema
name: Price Update Request
properties_list:
- description: New price amount.
  name: amount
  type: number
- description: Currency code (ISO 4217).
  name: currency
  type: string
provider_name: agilent-technologies
provider_slug: agilent-technologies
schema_file: json-schema/ilab-operations-api-price-update-request-schema.json
slug: ilab-operations-api-price-update-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/json-schema/ilab-operations-api-price-update-request-schema.json\",\n  \"title\": \"Price Update Request\",\n  \"description\": \"Request body for updating a service price.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"New price amount.\",\n      \"example\": 175.0\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code (ISO 4217).\",\n      \"example\": \"USD\"\n    }\n  },\n  \"required\": [\n    \"amount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/json-schema/ilab-operations-api-price-update-request-schema.json
tags:
- Life Sciences
- Diagnostics
- Laboratory
- Scientific Instruments
- LIMS
- Laboratory Automation
title: Price Update Request
---
