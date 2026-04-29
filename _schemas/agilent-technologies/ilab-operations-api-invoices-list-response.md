---
description: List of invoices for a core facility.
layout: schema
name: Invoices List Response
properties_list:
- description: ''
  name: invoices
  type: array
provider_name: agilent-technologies
provider_slug: agilent-technologies
schema_file: json-schema/ilab-operations-api-invoices-list-response-schema.json
slug: ilab-operations-api-invoices-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/json-schema/ilab-operations-api-invoices-list-response-schema.json\",\n  \"title\": \"Invoices List Response\",\n  \"description\": \"List of invoices for a core facility.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"invoices\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Invoice\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/json-schema/ilab-operations-api-invoices-list-response-schema.json
tags:
- Life Sciences
- Diagnostics
- Laboratory
- Scientific Instruments
- LIMS
- Laboratory Automation
title: Invoices List Response
---
