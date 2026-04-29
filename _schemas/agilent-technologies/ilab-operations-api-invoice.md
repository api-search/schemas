---
description: A billing invoice from a core facility.
layout: schema
name: Invoice
properties_list:
- description: Unique identifier for the invoice.
  name: id
  type: integer
- description: Billing period (YYYY-MM format).
  name: period
  type: string
- description: Current invoice status.
  name: status
  type: string
- description: Total invoice amount.
  name: total_amount
  type: number
- description: Currency code (ISO 4217).
  name: currency
  type: string
- description: Timestamp when the invoice was issued.
  name: issued_at
  type: string
provider_name: agilent-technologies
provider_slug: agilent-technologies
schema_file: json-schema/ilab-operations-api-invoice-schema.json
slug: ilab-operations-api-invoice
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/json-schema/ilab-operations-api-invoice-schema.json\",\n  \"title\": \"Invoice\",\n  \"description\": \"A billing invoice from a core facility.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the invoice.\",\n      \"example\": 300789\n    },\n    \"period\": {\n      \"type\": \"string\",\n      \"description\": \"Billing period (YYYY-MM format).\",\n      \"example\": \"2026-03\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current invoice status.\",\n      \"enum\": [\n        \"draft\",\n        \"sent\",\n        \"paid\",\n        \"voided\"\n      ],\n      \"example\": \"sent\"\n    },\n    \"total_amount\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n \
  \     \"description\": \"Total invoice amount.\",\n      \"example\": 2500.0\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code (ISO 4217).\",\n      \"example\": \"USD\"\n    },\n    \"issued_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the invoice was issued.\",\n      \"example\": \"2026-04-01T00:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/json-schema/ilab-operations-api-invoice-schema.json
tags:
- Life Sciences
- Diagnostics
- Laboratory
- Scientific Instruments
- LIMS
- Laboratory Automation
title: Invoice
---
